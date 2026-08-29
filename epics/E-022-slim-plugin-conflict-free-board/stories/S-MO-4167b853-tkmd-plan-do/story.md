---
id: S-MO-4167b853
type: story
title: Plan then implement with /tkmd-plan-do
status: backlog
priority: high
size: null
points: null
parent: E-022
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, commands, planning]
created: 2026-08-29
updated: 2026-08-29T10:55:00Z
started_at: null
completed_at: null
---

# S-MO-4167b853: Plan then implement with /tkmd-plan-do

## User story

As a Cursor user, I want `/tkmd-plan-do` so that one slash searches the board,
creates the smallest useful new work, and then implements those newly created
items without a second `/tkmd-do` invocation.

## Acceptance criteria

- [ ] The plugin exposes `/tkmd-plan-do` in addition to `/tkmd-init`, `/tkmd-plan`, `/tkmd-do`, and `/tkmd-commit`.
- [ ] The command runs the same planning behaviour as `/tkmd-plan`, then runs `/tkmd-do` only on the items that planning just created.
- [ ] If planning creates nothing (exact or overlapping match), implementation is skipped and the match is reported.
- [ ] `/tkmd-plan-do` never commits or pushes and never uses `in_progress`.
- [ ] Product docs and plugin READMEs describe the command without dropping the existing plan/do/commit loop.
