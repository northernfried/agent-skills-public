# Skills Index

Entry point for this skill library. Each category below is a directory of focused, reusable agent skill files.

## Responsibilities

- Host the master index for the shared skill set.
- Separate cross-cutting, reusable skills from project-specific configuration (which belongs in a project's own `CLAUDE.md` or equivalent).
- Provide stable categories for domain, platform, product, delivery, governance, template, and recipe content.

## Category Model

- `domains/`: domain-specific skills such as payments, pricing, compliance, and security.
- `platform/`: shared engineering and runtime skills for monorepo, tooling, testing, and infrastructure.
- `product/`: product overlays that are shared within a product family but don't belong in a single project's config.
- `delivery/`: planning, decomposition, QA, release, and workflow execution guidance.
- `governance/`: standards, controls, monitoring, and policy-oriented guidance.
- `templates/`: canonical authoring templates for new skills, recipes, and compliance chunks.
- `recipes/`: reusable procedure-style instructions with strong implementation guidance.

## Notable Skills

- `platform/api-builder.md` — designs/extends REST API contracts against the OpenAPI Specification and Google's API design guide (AIPs); orchestrates the `api-builder-*` sub-recipes in `recipes/`.
- `platform/llm-model-contract.md` — offline-first LLM provider abstraction pattern (tiers, resolution order, shared provider layer) for multi-app/agent codebases.
- `recipes/payment-processing-recipe.md` + `domains/pci-dss-req-3-4.md` — a worked example of linking a compliance requirement to a mandatory implementation recipe.
- `domains/agent-zero-trust-delegation.md` — a zero-trust skeleton for agent-to-application authorization: agents as a distinct principal, no inherited human entitlements, 15-30 minute delegation grants, and explicit defenses against an agent masquerading as the human it's acting for.
- `governance/github-push-sensitivity-review.md` — secret scanning, `.env`/`.env.example` conventions, structure-preserving placeholder values, and de-branding forked sample repos before a GitHub push.

## Adding a New Skill

1. Pick the right category above.
2. Start from a template in `templates/` (`skill-template.md`, `recipe-template.md`, or the builder templates).
3. Update the category's `README.md` and this file so the skill is discoverable.
