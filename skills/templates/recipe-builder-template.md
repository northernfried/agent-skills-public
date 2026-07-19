# Recipe Builder Template

Use this template to turn compliance notes, architecture guidance, or implementation practices into a new recipe quickly.

## 1. Intake Interview

Collect these answers before writing the recipe:

- **Working title:** What should the recipe be called?
- **Source type:** Is this based on policy, compliance guidance, a project, an activity/workflow, or a mix?
- **Primary purpose:** What must this recipe ensure or prevent?
- **Target audience:** Who must follow this recipe?
- **Compliance scope:** Which frameworks, policies, or controls apply?
- **Required controls:** What mandatory controls or guardrails must be included?
- **Firm standards:** What technical or operational standards must be followed?
- **Implementation context:** What systems, services, or workflows does this recipe affect?
- **Success criteria:** How will we know the recipe is complete and usable?
- **Example scenario:** What real-world case should the recipe cover?
- **Sources to credit:** Is there a document, team, or URL that should be referenced?

## 2. Recipe Blueprint

Fill in the following sections to create the new recipe.

### Recipe Name

[Insert recipe name]

### Overview

[Describe what the recipe covers and why it exists.]

### Required Compliance Frameworks

[List the specific compliance chunks, policies, or source documents that must be followed.]

- **Framework 1:** [Placeholder] -> See: [Link to source]
- **Framework 2:** [Placeholder] -> See: [Link to source]

### Firm Controls

[List the mandatory controls, security requirements, or architectural guardrails.]

- **Control ID [e.g., SEC-001]:** [Placeholder]
- **Control ID [e.g., ARCH-045]:** [Placeholder]

### Firm Standards

[List the specific technical, operational, or governance standards that support the controls.]

- **Standard 1:** [Placeholder]
- **Standard 2:** [Placeholder]

### Implementation Instructions

[Provide the step-by-step patterns, required actions, and implementation rules.]

1. [Step 1]
2. [Step 2]
3. [Step 3]

### Example Scenarios

[Add one or two realistic scenarios that show how this recipe should be applied.]

### Output / Deliverable

[Describe what a completed implementation should produce or what the recipe consumer should do.]

### Core Prompt / Instructions

```text
You are [role/expert persona] responsible for authoring a mandatory recipe.

Task:
Create a clear, source-grounded recipe that defines required controls, standards, and implementation instructions for [topic].

Use the following steps:
1. Confirm the scope and source materials.
2. Identify the mandatory compliance frameworks, controls, and standards.
3. Write implementation instructions that are specific, testable, and non-optional.

Guidelines:
- Do not invent controls or standards that are not supported by the source material.
- Keep the language firm, concise, and implementation-oriented.
- Make mandatory items explicit and easy to audit.

If key inputs are missing, ask for the smallest useful clarification before proceeding.
Prefer grounded, source-based reasoning over assumptions.
Return the result in the required recipe format.
```

### Quality Checklist

- [ ] The recipe scope is specific and easy to understand.
- [ ] Required frameworks and sources are clearly named.
- [ ] Mandatory controls are explicit and non-optional.
- [ ] Standards are concrete and testable.
- [ ] Instructions are actionable and implementation-ready.
- [ ] The recipe preserves compliance intent without adding unsupported requirements.

## 3. Governance Metadata

- **Recipe ID:** `REC-[0000]`
- **Owner:** [Team or role]
- **Version:** 1.0
- **Last Audited:** YYYY-MM-DD
- **Source Type:** [policy | compliance | project | activity | mixed]
- **Source URL:** [Optional source link]

## 4. Optional Fill-In Notes

Use this area to capture quick interview answers before finalizing the recipe.

- **Key source files or references:** [Placeholder]
- **Non-negotiable constraints:** [Placeholder]
- **Preferred tone:** [Placeholder]
- **Special cases:** [Placeholder]
- **Success signal:** [Placeholder]
