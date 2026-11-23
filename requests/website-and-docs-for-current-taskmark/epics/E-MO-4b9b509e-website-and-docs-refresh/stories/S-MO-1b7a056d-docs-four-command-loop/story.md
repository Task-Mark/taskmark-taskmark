---
id: S-MO-1b7a056d
type: story
title: Docs teach the four-command loop
status: backlog
priority: high
size: M
points: 5
parent: E-MO-4b9b509e
epic: E-MO-4b9b509e
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [docs, commands]
created: 2026-08-28
updated: 2026-08-28T23:15:25Z
started_at: null
completed_at: null
---

# S-MO-1b7a056d: Docs teach the four-command loop

## User story

As someone installing Taskmark, I want setup, commands, workflows, and the docs overview to describe only `/tkmd-init`, `/tkmd-create`, `/tkmd-do`, and `/tkmd-commit` so I can run the daily loop without leftover `/tsmk-*`, `/new-*`, or `/start-work` names.

## Acceptance criteria

- [ ] Docs overview, setup, commands, and workflows name exactly those four slashes and their real effects (init board + UI stubs; create new files only; do never commits and marks executed leaves done; commit is the only git entrypoint).
- [ ] `/tkmd-do` is documented as never using `in_progress` and as logging Prompt & feedback on a matching leaf (including a done leaf that still fits).
- [ ] `/tkmd-create` is documented as writing new item files only, with collision-resistant IDs; no “soft-attach to General” unless that reserved epic is still product behaviour.
- [ ] Searchable leftovers (`/tsmk`, `/new-epic`, `/create-task`, `/start-work`, `/commit-all`) are gone from current docs copy.
- [ ] Docs nav descriptions match this loop.
