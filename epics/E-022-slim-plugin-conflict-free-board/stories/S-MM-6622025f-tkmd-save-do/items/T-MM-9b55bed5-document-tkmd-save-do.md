---
id: T-MM-9b55bed5
type: task
title: Document /tkmd-save-do in website docs
status: done
priority: medium
size: S
points: 3
parent: S-MM-6622025f
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [docs, commands, website]
created: 2026-08-31
updated: 2026-08-31T12:29:40Z
started_at: 2026-08-31T12:23:49Z
completed_at: 2026-08-31T12:29:40Z
---

# T-MM-9b55bed5: Document /tkmd-save-do in website docs

## Description

Teach `/tkmd-save-do` on the public site so visitors see it as save-then-do
after Cursor Plan mode, not a replacement for `/tkmd-save` or `/tkmd-do`.
Update the commands reference, docs nav, and any slash-set copy on setup,
workflows, overview, and related pages that would otherwise omit the new slash.

## Acceptance criteria

- [x] `/docs/commands` lists `/tkmd-save-do` with purpose: save like `/tkmd-save`, then implement the newly created items like `/tkmd-do`.
- [x] Setup, workflows, overview, and specification mention when to use `/tkmd-save-do` versus save-only then do later.
- [x] Docs still state that `/tkmd-commit` is the only command that commits and that `/tkmd-save-do` never commits.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T12:23:49Z | prompt | Marco Mendão | `/tkmd-plan-do`: create `/tkmd-save-do`, similar to `/tkmd-save`, that saves a Cursor plan and then immediately executes the tasks that plan generated. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T12:23:49Z | 2026-08-31T12:26:01Z | Documented `/tkmd-save-do` on commands, setup, workflows, overview, and specification. |
