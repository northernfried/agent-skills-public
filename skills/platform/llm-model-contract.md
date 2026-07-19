# Skill Name: Offline-First LLM Model Contract

## 🎯 Objective

A reusable architecture pattern for multi-app / multi-agent codebases: applications never hard-code a provider or model name. Instead they declare a requirement on an **LLM source** and ask for a capability **tier**, so the same app runs unmodified against a local model, a self-hosted endpoint, or a hosted API, and degrades gracefully when offline.

## 👤 Target Persona

Platform/infra engineer building shared LLM-access infrastructure for more than one service or agent, who wants to avoid every app re-implementing provider selection, key handling, and fallback logic independently.

## 📥 Inputs Required

- **Provider set:** which LLM sources must be supported (e.g. a local runtime like Ollama, plus one or more hosted APIs)
- **Tiering needs:** does the workload split cleanly into cost/latency tiers (cheap classification vs. general reasoning vs. long-context/hard reasoning)?
- **Deployment shape:** monorepo with a shared package, or independently-packaged apps that must still work standalone?
- **Offline requirement:** must the app function with zero internet access, or are hosted providers acceptable as the default?

## 📤 Expected Output

- A small `require_llm_source()`-style entry point apps call once at startup
- A resolution order (package default → manifest file → environment variables) so both zero-config and fully-overridden deployments work
- A shared provider layer (one module per provider) that individual apps consume, never reimplement

## 🤖 Core Prompt / Instructions

```text
You are a platform engineer designing an LLM access layer shared across
multiple applications. Apply this contract:

1. THE CONTRACT
   Apps never hard-code a provider or model name. They call one function
   (e.g. `require_llm_source()`) at startup, which:
   - resolves which source to use (local runtime, self-hosted endpoint, or
     hosted API) via a defined precedence order
   - verifies the source is actually usable (endpoint reachable, required
     models installed, or API key present for hosted kinds)
   - raises a clear, actionable error with remediation steps if not usable
     ("fail fast, with instructions" — not a mysterious failure on the first
     real model call)

2. TIERS, NOT MODEL NAMES
   Define 2-3 capability tiers (e.g. fast / primary / heavy) each mapped to a
   default model per provider. Application code asks for a tier
   (`source.model_for("primary")`), never a literal model string — this is
   the one place model choice changes when the underlying catalog drifts.

3. RESOLUTION ORDER (lowest to highest precedence)
   a. Package defaults baked into the shared library — an app packaged and
      distributed independently still works offline against a local runtime
      with zero configuration.
   b. A manifest file (e.g. `models.toml`), resolved via an env var override
      or by walking up from the working directory to a canonical location.
   c. Environment variables — the bring-your-own-source path for end users:
      SOURCE_KIND, BASE_URL, API_KEY, and per-tier model overrides.

4. SHARED PROVIDER LAYER
   Put the concrete provider implementations (one local runtime adapter, one
   per hosted API, one generic OpenAI-compatible adapter) in a shared
   package, not duplicated per app. Include: an injected settings/secrets
   store (so it can run standalone with in-memory defaults, or wired into a
   real DB by a consuming app), a health/circuit-breaker layer, usage
   tracking, and a redacting `to_dict()`/logging helper so API keys never hit
   logs.

5. APP-SPECIFIC PERSISTENCE IS INJECTED, NEVER IMPORTED
   Each consuming app wires its own settings DB / usage table / audit log
   into the shared registry; the shared package itself stays app-agnostic
   with working in-memory defaults so new apps get a functioning registry
   with zero wiring.

6. RULES OF THUMB
   - One local runtime instance shared by all apps/containers — no per-app
     duplicate model stores or volumes.
   - Offline-first: the local source is the default; hosted providers are
     optional enhancements, and the app must degrade gracefully with no
     internet.
   - Change models in exactly one place (the manifest / package default),
     and verify against the runtime's actual installed catalog before
     changing defaults — installed model catalogs drift over time.
   - Never log a raw API key.
```

## ✅ Success Criteria / Quality Checklist

- [ ] No application code contains a literal model name — only tier requests
- [ ] A freshly packaged/independent copy of an app still boots offline against a local runtime with zero configuration
- [ ] Startup fails fast with actionable remediation text if no usable source is configured, rather than failing on the first model call
- [ ] Provider implementations live in one shared location, not duplicated per app
- [ ] API keys are never written to logs (verified via the redacting log helper)

---
**Metadata**
- **Version:** 1.0
- **Last Updated:** 2026-07-19
- **Author:** northernfried
