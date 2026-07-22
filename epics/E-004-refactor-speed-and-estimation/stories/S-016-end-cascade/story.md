---
id: S-016
type: story
title: End cascade for task, story, epic
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 9
points_source: rolled_up
estimate_minutes: 150
actual_minutes: 144
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-004
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [complete-work, cascade, status]
created: 2026-07-21
updated: 2026-07-22T00:30:21.269Z
started_at: 2026-07-21T20:43:27Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 8640000
---
# S-016: End cascade for task, story, epic

## User story

As a user or agent, I want an end/complete action so items get completed_at, and completing the last open child closes the parent story or epic.

## Acceptance criteria

- [x] End/complete action sets completed_at and closes open work sessions.
- [x] When all child tasks of a story are done/cancelled (and at least one done), story completes.
- [x] When all child stories of an epic are done/cancelled (and at least one done), epic completes.
- [x] Skills/conventions updated; sync-status derives the same cascade.

## Tasks

- [T-042: End/complete sets completed_at and closes sessions](items/T-042-end-item-sets-completed-at.md)
- [T-043: Cascade complete parents when last child ends](items/T-043-cascade-complete-parents.md)
- [T-044: Update complete-work skills and conventions](items/T-044-update-complete-skills-conventions.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T22:56:48Z | prompt | Create epic: refactor speed/estimation — 1-month velocity, start/end cascade, dual effort vs actual |
| 2 | 2026-07-21T23:07:27Z | feedback | E-004 dual model delivered |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T20:43:27Z | 2026-07-21T23:07:27Z | auto-backfilled: velocity × points (missing work log) |

