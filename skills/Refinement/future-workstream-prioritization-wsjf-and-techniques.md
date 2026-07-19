# Skill Name: Future Workstream Prioritization (WSJF + Multi-Technique Toolkit)

## 🎯 Objective

Prioritizes future workstreams using SAFe WSJF as the default economic sequencing method, while documenting and selectively applying additional Agile prioritization techniques when data quality, urgency, or context requires a different lens.

Enforces strategy-first category allocation so prioritization is constrained by explicit capacity shares across:

- Revenue Generation
- Revenue Protection
- Platform Stability

## 👤 Target Persona

Product Manager, Product Owner, Program Manager, Portfolio Lead, Engineering Manager

## 📚 Required Sources

- **SAFe WSJF reference:** [Weighted Shortest Job First](https://framework.scaledagile.com/wsjf/)
- **Technique catalog reference:** [8 Best Prioritization Models in Agile](https://fibery.com/blog/product-management/agile-prioritization-techniques/)
- **Prioritization framework reference:** [Six product prioritization frameworks and how to pick the right one](https://www.atlassian.com/agile/product-management/prioritization-framework)

## 📥 Inputs Required

- **Future Workstream Candidates:** Epics/initiatives/options under consideration.
- **Category Mapping (Required):** Each candidate must be mapped to one primary category (Revenue Generation, Revenue Protection, or Platform Stability).
- **Capacity Allocation Policy (Required):** Planned share per category for the increment (default example: 50% / 30% / 20%).
- **Economic Signals:** Relative user-business value, time criticality, risk reduction or opportunity enablement.
- **Delivery Signals:** Relative job size/duration, dependency load, and constraint windows.
- **Context Signals:** Urgency, confidence level of data, stakeholder alignment complexity.
- **Planning Window:** Program increment, quarter, or equivalent horizon.

## 📤 Expected Output

- Ranked workstream list with explicit prioritization method(s) used.
- Category-level ranked lists (ranked within each category first).
- WSJF-based sequencing for candidates with sufficient data.
- Technique-selection rationale when alternatives to WSJF are used.
- Capacity-fit decision per category (fits / exceeds / deferred).
- Combined increment sequence across all categories after in-category prioritization.
- Trade-off notes and assumptions for decisions.
- Explicit over-capacity deferrals when category capacity is full.
- Exception list for leadership-approved over-capacity inclusions.
- Recommended review cadence and reprioritization triggers.

## 🤖 Core Prompt / Instructions

```text
You are a portfolio refinement analyst prioritizing future workstreams.

Default to SAFe WSJF for sequencing workstreams with adequate economic and size data.
Use alternative techniques only when context suggests they are a better fit.
Prioritization must be strategy-driven and capacity-constrained by category.

I will provide workstream candidates and planning context.

Produce the result in this order:
1. Confirm planning horizon, candidate set, and category capacity policy.
2. Validate every candidate has one primary category:
   - Revenue Generation
   - Revenue Protection
   - Platform Stability
3. Prioritize within each category first using WSJF where data is sufficient:
   - explain numerator factors (value, time criticality, risk reduction/opportunity enablement)
   - explain denominator factor (relative job size/duration)
   - provide ranked sequencing with rationale for each category
4. If WSJF inputs are weak or incomplete, choose one supplemental method and explain why:
   - MoSCoW
   - Kano
   - Priority Poker
   - 100-dollar test (cumulative voting)
   - Cost of Delay (CoD)
   - Business value vs effort (ROI)
   - RICE
   - Value vs effort matrix
   - Opportunity scoring
5. Apply category capacity gates (for example 50/30/20 shares):
   - admit only work that fits remaining category capacity
   - mark excess work as deferred to next increment
6. Create overall combined increment sequence across all categories from admitted work.
7. Compare outputs when multiple methods are used and reconcile conflicts.
8. Provide final prioritized order with confidence level and key assumptions.
9. List what new data would most improve prioritization confidence.
10. Define when to re-run prioritization (trigger-based, not calendar-only).
11. Produce a leadership exception section for any over-capacity item and why it was approved.

Rules:
- Use WSJF as the default, not the only method.
- Strategy alignment is the primary driver before scoring methods are applied.
- Prioritization is category-first, then combined for increment execution.
- Do not admit new work to an increment when category capacity is full unless leadership explicitly approves an exception.
- Never hide uncertainty; mark low-confidence inputs clearly.
- Prioritize sequencing decisions over static ranking.
- Capture trade-offs explicitly when methods disagree.
- Keep outputs decision-ready for portfolio/workstream planning.
```

## Technique Selection Guide

Use this practical selection logic:

- **WSJF:** Best default when relative value, urgency, risk reduction, and job size are available.
- **MoSCoW:** Fast triage when data is sparse and immediate grouping is needed.
- **Kano:** Useful when customer satisfaction and delight trade-offs are central.
- **Priority Poker / 100-dollar test:** Useful for rapid team alignment and stakeholder participation.
- **CoD / ROI:** Useful when financial impact is dominant and estimable.
- **RICE:** Useful when reach/impact/confidence/effort data is available and decisions need stronger analytics.
- **Value vs effort matrix:** Useful for fast visual trade-offs when impact and effort can be estimated quickly.
- **Opportunity scoring:** Useful when customer importance and satisfaction data are available and gaps should drive prioritization.

## ✅ Success Criteria / Quality Checklist

- [ ] Every item is mapped to one prioritization category.
- [ ] Category capacity allocation is explicit for the increment (for example 50/30/20).
- [ ] Prioritization is completed within categories before overall sequence is produced.
- [ ] Over-capacity items are deferred unless leadership exception is explicitly documented.
- [ ] WSJF is attempted first and documented when feasible.
- [ ] Alternative method choice is justified by context and data quality.
- [ ] Final ranking includes confidence and assumptions.
- [ ] Trade-offs and disagreements between methods are visible.
- [ ] Reprioritization triggers are explicitly defined.

---

## Metadata

- **Version:** 1.0
- **Last Updated:** 2026-07-19
- **Author:** Workspace Refinement Skills
