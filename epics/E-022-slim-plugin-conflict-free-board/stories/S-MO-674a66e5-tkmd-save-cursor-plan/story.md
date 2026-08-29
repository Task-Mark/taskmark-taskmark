---
id: S-MO-674a66e5
type: story
title: Save Cursor Plan mode plans with /tkmd-save
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
tags: [plugin, commands, planning, cursor-plan]
created: 2026-08-29
updated: 2026-08-29T10:58:33Z
started_at: null
completed_at: null
---

# S-MO-674a66e5: Save Cursor Plan mode plans with /tkmd-save

## User story

As a Cursor user who just finished Plan mode, I want `/tkmd-save` so that the
approved plan is turned into Taskmark epics, stories, tasks, and bugs—with the
plan’s diagrams and other visual aids kept on the work items—without retyping
the plan as prose for `/tkmd-plan`.

## Acceptance criteria

- [ ] The plugin exposes `/tkmd-save` alongside the other `/tkmd-*` commands.
- [ ] The command reads the Cursor Plan mode plan from the current session (or the plan the user points at) and decomposes it with the same hierarchy rules as `/tkmd-plan` (epic / story / task / bug, dedupe, new files only).
- [ ] Graphics, diagrams, and other visual supports from the plan appear in the work items that `/tkmd-save` creates (linked or embedded where the board markdown allows).
- [ ] `/tkmd-save` never commits, never pushes, and never uses `in_progress`.
- [ ] Product docs and plugin READMEs describe when to run `/tkmd-save` after Plan mode versus writing free-form `/tkmd-plan` prose.
