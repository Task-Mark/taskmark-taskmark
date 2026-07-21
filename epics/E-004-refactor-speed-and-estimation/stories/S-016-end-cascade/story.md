---
id: S-016
type: story
title: End cascade for task, story, epic
status: backlog
priority: high
size: L
size_source: suggested
size_basis: [T-042, T-043, T-044]
points: 9
points_source: suggested
estimate_minutes: 1440
actual_minutes: 0
estimate_basis: [T-042, T-043, T-044]
session_cap_minutes: 480
parent: E-004
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [complete-work, cascade, status]
created: 2026-07-21
updated: 2026-07-21T22:56:48Z
started_at: null
completed_at: null
---

# S-016: End cascade for task, story, epic

## User story

As a user or agent, I want an end/complete action so items get completed_at, and completing the last open child closes the parent story or epic.

## Acceptance criteria

- [ ] End/complete action sets completed_at and closes open work sessions.
- [ ] When all child tasks of a story are done/cancelled (and at least one done), story completes.
- [ ] When all child stories of an epic are done/cancelled (and at least one done), epic completes.
- [ ] Skills/conventions updated; sync-status derives the same cascade.

## Tasks

- [T-042: End/complete sets completed_at and closes sessions](items/T-042-end-item-sets-completed-at.md)
- [T-043: Cascade complete parents when last child ends](items/T-043-cascade-complete-parents.md)
- [T-044: Update complete-work skills and conventions](items/T-044-update-complete-skills-conventions.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T22:56:48Z | prompt | Create epic: refactor speed/estimation — 1-month velocity, start/end cascade, dual effort vs actual |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

