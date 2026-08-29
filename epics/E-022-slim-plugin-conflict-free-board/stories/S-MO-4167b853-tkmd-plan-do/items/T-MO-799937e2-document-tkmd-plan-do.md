---
id: T-MO-799937e2
type: task
title: Document /tkmd-plan-do in website docs
status: done
priority: medium
size: S
points: 3
parent: S-MO-4167b853
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

# T-MO-799937e2: Document /tkmd-plan-do in website docs

## Description

Teach `/tkmd-plan-do` on the public site so visitors see it as plan-then-do,
not a replacement for `/tkmd-plan` or `/tkmd-do`. Update the commands
reference, docs nav, and any “exactly four commands” copy on setup, workflows,
overview, and landing that would otherwise omit the new slash.

## Acceptance criteria

- [x] `/docs/commands` lists `/tkmd-plan-do` with purpose: plan like `/tkmd-plan`, then implement the newly created items like `/tkmd-do`.
- [x] Docs nav and metadata no longer claim the plugin exposes only four commands.
- [x] Setup, workflows, and docs overview mention when to use `/tkmd-plan-do` versus plan-only then do later.
- [x] The page still states that `/tkmd-commit` is the only command that commits and that `/tkmd-plan-do` never commits.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:55:00Z | prompt | Marco Mendão | Add `/tkmd-plan-do`: same as `/tkmd-plan`, then run `/tkmd-do` on the tasks just created. |
| 2026-08-29T11:09:00Z | prompt | Marco Mendão | `/tkmd-do`: implement every backlog work item under epic E-022. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:09:00Z | 2026-08-29T11:09:44Z | Documented `/tkmd-plan-do` on commands, setup, workflows, and overview. |
