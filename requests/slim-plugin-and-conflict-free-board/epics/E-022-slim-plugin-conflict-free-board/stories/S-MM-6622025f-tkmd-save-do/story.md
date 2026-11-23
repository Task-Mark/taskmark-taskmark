---
id: S-MM-6622025f
type: story
title: Save then implement with /tkmd-save-do
status: backlog
priority: high
size: null
points: null
parent: E-022
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, commands, planning, cursor-plan]
created: 2026-08-31
updated: 2026-08-31T12:23:49Z
started_at: null
completed_at: null
---

# S-MM-6622025f: Save then implement with /tkmd-save-do

## User story

As a Cursor user who just finished Plan mode, I want `/tkmd-save-do` so that
one slash turns that plan into Taskmark items and then implements only those
newly created items, without a second `/tkmd-do` invocation.

## Acceptance criteria

- [ ] The plugin exposes `/tkmd-save-do` alongside `/tkmd-save` and the other `/tkmd-*` commands.
- [ ] The command runs the same save behaviour as `/tkmd-save`, then runs `/tkmd-do` only on the items that save just created.
- [ ] If save creates nothing (exact or overlapping match), implementation is skipped and the match is reported.
- [ ] `/tkmd-save-do` never commits or pushes and never uses `in_progress`.
- [ ] Product docs and plugin READMEs describe when to use `/tkmd-save-do` versus save-only then do later.
