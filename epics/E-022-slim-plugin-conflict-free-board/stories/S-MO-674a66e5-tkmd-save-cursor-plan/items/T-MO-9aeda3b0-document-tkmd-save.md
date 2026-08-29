---
id: T-MO-9aeda3b0
type: task
title: Document /tkmd-save in website docs
status: done
priority: medium
size: S
points: 3
parent: S-MO-674a66e5
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [docs, commands, website]
created: 2026-08-29
updated: 2026-08-29T11:14:10Z
started_at: 2026-08-29T11:09:00Z
completed_at: 2026-08-29T11:14:10Z
---

# T-MO-9aeda3b0: Document /tkmd-save in website docs

## Description

Document `/tkmd-save` on the public site as the post–Plan mode path: read the
Cursor plan, create Taskmark hierarchy, keep diagrams/visuals on the new items.
Clarify how it differs from free-form `/tkmd-plan` and from `/tkmd-plan-do`.

## Acceptance criteria

- [x] `/docs/commands` lists `/tkmd-save` with purpose: after Cursor Plan mode, turn the plan into epic/story/task/bug items and carry plan visuals into those items.
- [x] Setup, workflows, and overview describe when to use `/tkmd-save` versus `/tkmd-plan` (prose) versus `/tkmd-plan-do` (plan then implement).
- [x] Docs state that `/tkmd-save` never commits and that `/tkmd-commit` remains the only commit command.
- [x] Command-count / “four commands only” copy is updated wherever it would omit `/tkmd-save`.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:58:33Z | prompt | Marco Mendão | Add `/tkmd-save` after Cursor Plan mode: split the plan into epic/story/task/bug work items and keep plan diagrams/visuals on those items. |
| 2026-08-29T11:09:00Z | prompt | Marco Mendão | `/tkmd-do`: implement every backlog work item under epic E-022. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:09:00Z | 2026-08-29T11:09:44Z | Documented `/tkmd-save` on commands, setup, workflows, overview, and landing. |
