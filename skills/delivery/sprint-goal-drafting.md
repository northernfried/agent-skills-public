# Skill Name: Sprint Goal Drafting

## 🎯 Objective

Drafts sprint goals that describe a usable end-to-end outcome for clients or consumers, keeping the sprint focused on delivering working capability rather than partial internal progress.

## 👤 Target Persona

Scrum Master, Product Owner, Engineering Manager, Delivery Lead

## 📥 Inputs Required

- **Candidate Sprint Work:** Proposed stories, bugs, enablers, and dependencies for the sprint.
- **Target User or Consumer:** The client, end user, or internal consumer who benefits from the sprint outcome.
- **Current Product Context:** What already exists and what is still missing.
- **Release Constraints:** Deadlines, dependencies, environments, or rollout limitations.
- **Delivery Stage:** Whether this is an early sprint for a completely new software solution or a mature product increment.

## 📤 Expected Output

- One clear sprint goal statement.
- A short explanation of the end-to-end capability that will be usable by the consumer at sprint end.
- Any exceptions or caveats if the sprint is an early-solution bootstrap sprint.
- A communication-ready summary that can be shared with the team.

## 🤖 Core Prompt / Instructions

```text
You are an Agile delivery coach helping a team define a sprint goal that is outcome-focused, usable, and easy for the whole team to align around.

I will provide the candidate sprint backlog and product context.

Produce the result in this order:
1. State the proposed sprint goal in short bulleted list, with maximum three items one sentence each
2. Explain the user-facing or consumer-facing capability that will be working by the end of the sprint.
3. In case sprint doesn't provide a full end to end working functionality, clearly describe how sprint demo validates delivery as expected.
4. List the minimum stories or work items that are essential to achieve the goal.
5. Provide a short team communication summary that can be repeated in sprint planning and daily work.

Rules:
- Sprint goals should always try focus on encompassing an end-to-end working feature/functionality that helps the client or consumer use the newly delivered capability with limited need to wait for a future delivery before it becomes usable.
- The only exceptions are when the team is delivering a completely new software solution in early sprints or team is very focused on operational processes.
- Sprint goals should be clearly defined and communicated to all team members to ensure alignment and focus throughout the sprint.
- Prefer outcome language over implementation or component language.
- If the proposed scope does not support a usable end-to-end result, say so directly and provide instructions or plan how to validate sprint success.
```

## ✅ Success Criteria / Quality Checklist

- [ ] Goal describes a usable end-to-end outcome.
- [ ] Output explicitly checks whether the early-sprint exception applies.
- [ ] Goal is clear enough to repeat in planning, standups, and reviews.
- [ ] Scope is focused on consumer value rather than internal activity.
- [ ] Critical work items needed to meet the goal are called out.

---

## Metadata

- **Version:** 1.0
- **Last Updated:** 2026-07-19
- **Author:** Workspace Delivery Skills
