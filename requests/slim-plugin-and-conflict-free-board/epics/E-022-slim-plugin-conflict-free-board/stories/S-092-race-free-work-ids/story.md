---
id: S-092
type: story
title: Collision-resistant work item IDs
status: backlog
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 13
points_source: rolled_up
estimate_minutes: 130
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-022
epic: E-022
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, collaboration, board]
created: 2026-08-28
updated: 2026-08-28T12:37:43.783Z
started_at: null
completed_at: null
actual_ms: 0
---

# S-092: Collision-resistant work item IDs

## User story

As two people creating tasks at once, I want IDs that cannot collide so we do not allocate the same T-NNN.

## Acceptance criteria

- [ ] New tasks/bugs/stories/epics do not use a single global sequential counter that two clones can duplicate.
- [ ] IDs remain unique board-wide and parseable by the UI.
- [ ] Convention docs and sample board describe the new scheme.

## Tasks

- [T-297: Replace sequential global T-NNN allocation](items/T-297-collision-resistant-id-allocator.md)
- [T-298: Update conventions, UI, and samples for the new IDs](items/T-298-migrate-id-docs-and-ui.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-28T12:19:14Z | prompt | Marco Mendão | Full housekeeping: slim commands, drop derived board files, static sizing, leaf-only MD, new IDs, delete unused plugin pieces. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
