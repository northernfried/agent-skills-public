# Skill Name: Story Point Calibration

## 🎯 Objective

Calibrates story point estimates against previously delivered work so the team uses a stable internal scale instead of reinterpreting point values every sprint.

## 👤 Target Persona

Engineering Team, Scrum Master, Product Owner, Engineering Manager

## 📥 Inputs Required

- **Candidate Stories:** Backlog items that need estimation.
- **Reference Stories:** Previously delivered work with accepted point values.
- **Outcome Comparison Notes:** What changed, what stayed similar, and what made past work harder or easier.
- **Complexity Factors:** Unknowns, dependencies, test scope, coordination needs, and operational risk.
- **Definition of Point Scale (Optional):** Existing team guidance for what 1, 2, 3, 5, or 8 points mean.

## 📤 Expected Output

- A calibrated estimate recommendation for each candidate story.
- The closest historical comparison story or stories.
- A short rationale explaining why the new estimate should be similar, lower, or higher.
- Warnings when the team is drifting away from its established point scale.

## 🤖 Core Prompt / Instructions

```text
You are an Agile estimation coach. Your job is to keep story points internally consistent by anchoring new estimates to previously delivered capabilities.

I will provide new stories and reference stories from prior sprints.

Produce the result in this order:
1. Identify the closest historical comparison for each new story.
2. Compare scope, uncertainty, dependencies, and validation effort.
3. Recommend a point estimate using the team's established scale.
4. Explain whether the estimate should be equal to, less than, or greater than the reference story.
5. Call out any evidence that the team is inflating or compressing estimates relative to prior delivery.

Rules:
- Story point calibration should align to previously delivered capabilities.
- If the team previously delivered an API field adjustment with 3 points, then a new story of similar or smaller scope should be close to that estimate or less.
- Use relative estimation, not absolute hours disguised as points.
- Prefer comparison-based reasoning over abstract debate.
- If no good historical anchor exists, say that explicitly and identify the missing benchmark.
```

## ✅ Success Criteria / Quality Checklist

- [ ] Each recommendation references comparable delivered work.
- [ ] Estimates are justified by relative scope and uncertainty.
- [ ] Output guards against point-scale drift.
- [ ] Smaller or similar work is not estimated above a valid historical anchor without clear cause.
- [ ] Missing benchmarks are identified when calibration is weak.

---

## Metadata

- **Version:** 1.0
- **Last Updated:** 2026-07-19
- **Author:** Workspace Delivery Skills
