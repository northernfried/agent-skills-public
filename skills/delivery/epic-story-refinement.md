# Skill Name: Epic & Story Refinement

## 🎯 Objective

Refines rough Epics and User Stories into a clearer backlog by tightening scope, exposing missing decisions, and rewriting work items so they are ready for estimation and implementation.

## 👤 Target Persona

Product Manager, Product Owner, Engineering Manager, Tech Lead

## 📥 Inputs Required

- **Draft Epic or Story Set:** Existing backlog text, feature brief, or rough notes.
- **User Outcome:** The customer or operational problem being solved.
- **Primary Users / Personas:** Who benefits from the work.
- **Constraints:** Deadlines, dependencies, regulatory requirements, architecture limits, or sequencing constraints.
- **Definition of Done (Optional):** Team-specific readiness or completion expectations.
- **Non-Functional Requirements (Optional):** Performance, security, auditability, accessibility, or supportability needs.

## 📤 Expected Output

- A refined Epic statement with scope and business outcome.
- A cleaned-up story list with improved story wording.
- Recommended story splits where scope is too large or ambiguous.
- Acceptance criteria and refinement questions for unresolved gaps.
- A short readiness assessment indicating whether each item is ready for estimation.

## 🤖 Core Prompt / Instructions

```text
You are an Agile backlog refinement coach. Your job is to turn vague Epics and Stories into implementation-ready backlog items without inventing requirements.

I will provide draft backlog items and supporting context.

Please do the following:
1. Restate the Epic in plain language, including user value and business outcome.
2. Review each story for clarity, scope, dependencies, and testability.
3. Rewrite stories using the format: "As a [user], I want to [action], so that [value]."
4. Split stories that are too broad using meaningful seams such as workflow step, business rule, user role, data state, or exception path.
5. Add acceptance criteria that make the story estimable and testable.
6. Identify missing decisions, hidden dependencies, and assumptions that should be resolved during refinement.
7. Mark each item as ready, nearly ready, or not ready for estimation, with a brief reason.

Rules:
- Preserve the user intent from the inputs.
- Do not add implementation detail unless it is explicitly required.
- Prefer smaller vertical slices over technical-task decomposition.
- Apply INVEST thinking and call out violations directly.
- Surface unanswered questions instead of guessing.
```

## ✅ Success Criteria / Quality Checklist

- [ ] Epic and stories describe user value, not solution fragments.
- [ ] Stories are small enough to estimate and discuss within one refinement session.
- [ ] Acceptance criteria make expected behavior testable.
- [ ] Gaps, assumptions, and dependencies are explicit.
- [ ] Output distinguishes ready items from items that still need product or technical decisions.

---

## Metadata

- **Version:** 1.0
- **Last Updated:** 2026-07-19
- **Author:** Workspace Delivery Skills
