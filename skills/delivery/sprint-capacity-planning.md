# Skill Name: Sprint Capacity Planning

## 🎯 Objective

Calculates realistic team capacity for the next sprint by separating raw availability from delivery capacity and translating that into a planning recommendation.

## 👤 Target Persona

Scrum Master, Engineering Manager, Product Owner, Delivery Lead

## 📥 Inputs Required

- **Sprint Dates:** Start and end dates for the upcoming sprint.
- **Team Roster:** Names, roles, and expected participation for each team member.
- **Availability Adjustments:** Planned leave, holidays, onboarding, part-time schedules, or other known time away.
- **Non-Feature Load:** Support rotation, incidents, meetings, ceremonies, maintenance, and platform work.
- **Historical Delivery Data (Optional):** Velocity from the last 3-5 sprints, completed story points, or completed ticket counts.
- **Work Intake Constraints (Optional):** Known dependencies, blocked work, or hard deadlines.

## 📤 Expected Output

- A capacity summary table by team member and for the full sprint.
- Explicit assumptions used in the calculation.
- A recommended planning range such as conservative, target, and stretch capacity. Including uncertainty range indicators (known normal drift experience by team due to production incidents, distractions and similar topics)
- Risks that may reduce actual delivery capacity.

## 🤖 Core Prompt / Instructions

```text
You are an Agile delivery coach helping a software team plan the next sprint using realistic capacity, not wishful allocation.

I will provide sprint dates, team members, expected availability, non-feature work, and optionally historical delivery data.

Produce the result in this order:
1. Summarize the planning assumptions.
2. Calculate raw person-days or person-hours available for each team member.
3. Subtract known reductions such as leave, holidays, ceremonies, support load, interrupts, and recurring maintenance.
4. Convert the remaining time into effective delivery capacity, calling out any focus-factor assumptions.
5. Compare the result against historical delivery data if provided.
6. Recommend a conservative, target, and stretch sprint capacity.
7. List the top risks, unknowns, and follow-up questions before sprint commitment.

Rules:
- Do not treat every available hour as feature delivery time.
- Distinguish clearly between availability, capacity, and forecast.
- Prefer a range over a single exact number when uncertainty is material.
- Flag when historical velocity conflicts with the calculated capacity.
- State assumptions explicitly instead of hiding them in the math.

If the inputs are incomplete, identify the minimum missing data needed to make the estimate credible.
```

## ✅ Success Criteria / Quality Checklist

- [ ] Capacity accounts for leave, ceremonies, and interrupt-driven work.
- [ ] Output clearly separates availability from forecasted delivery.
- [ ] Assumptions and confidence level are explicit.
- [ ] Recommendation avoids false precision and provides a usable planning range.
- [ ] Risks and missing inputs are surfaced before commitment.

---

## Metadata

- **Version:** 1.0
- **Last Updated:** 2026-07-19
- **Author:** Workspace Delivery Skills
