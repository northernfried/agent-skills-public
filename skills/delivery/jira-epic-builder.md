# Skill Name: Jira Epic & Story Builder

## 🎯 Objective
Translates high-level business requirements or a feature brief into structured Jira Epics, complete with nested User Stories and Acceptance Criteria (BDD format).

## 👤 Target Persona
Product Owner, Technical Product Manager

## 📥 Inputs Required
- **Feature Brief:** A paragraph or document explaining what needs to be built and why.
- **Technical Context (Optional):** Any known architectural constraints or specific systems involved.

## 📤 Expected Output
- 1 Epic Title and Description (including Business Value).
- 3-5 User Stories.
- Gherkin-style Acceptance Criteria (Given/When/Then) for each User Story.

## 🤖 Core Prompt / Instructions
```text
You are an Agile Product Owner expert in writing clear, actionable Jira tickets for engineering teams.
I will provide you with a [Feature Brief].

Break this feature down into an Agile structure:
1. **Epic:** Write a concise Epic title and a description that clearly states the user value and business goal.
2. **User Stories:** Break the Epic down into mutually exclusive, collectively exhaustive User Stories using the format: "As a [User], I want to [Action], so that [Value/Reason]."
3. **Acceptance Criteria:** For every User Story, write 2-3 Acceptance Criteria using the BDD format (Given [Context], When [Action], Then [Result]).

Ensure the stories are granular enough to be estimated by an engineering team. Do not include implementation details unless specified in the inputs.
```

## ✅ Success Criteria / Quality Checklist
- [ ] Stories follow the INVEST principle (Independent, Negotiable, Valuable, Estimable, Small, Testable).
- [ ] Acceptance Criteria cover both happy paths and edge cases.
- [ ] The Epic captures the overall business value clearly.

---
**Metadata**
- **Version:** 1.0
- **Last Updated:** 2024-05-20
- **Author:** PM Team
