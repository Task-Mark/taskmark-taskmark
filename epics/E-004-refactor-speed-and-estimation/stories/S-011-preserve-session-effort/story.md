---
id: S-011
type: story
title: Preserve session effort tracking
status: done
priority: high
size: S
size_source: rolled_up
size_basis: [sum:tasks]
points: 3
points_source: rolled_up
estimate_minutes: 136
actual_minutes: 2
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-004
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [effort, work-log, conventions]
created: 2026-07-21
updated: 2026-07-21T23:18:07Z
started_at: 2026-07-21T23:05:18Z
completed_at: 2026-07-21T23:07:27Z
---
# S-011: Preserve session effort tracking

## User story

As a team using Taskmark, I want AI/human session elapsed time still stored so we keep effort history even as actual meaning changes.

## Acceptance criteria

- [x] Work log sessions continue to record Started/Ended and billable elapsed minutes.
- [x] Session effort is retained as a first-class signal (documented field name, e.g. effort_minutes or work-log-derived).
- [x] Conventions clarify effort (sessions) vs actual (start→complete).

## Tasks

- [T-030: Document effort vs actual dual model](items/T-030-document-effort-vs-actual.md)
- [T-031: Keep work-log session effort computation](items/T-031-keep-work-log-effort.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T23:05:18Z | prompt | develop the epic E-004 |
| 1 | 2026-07-21T22:56:48Z | prompt | Create epic: refactor speed/estimation — 1-month velocity, start/end cascade, dual effort vs actual |
| 2 | 2026-07-21T23:07:27Z | feedback | E-004 dual model delivered |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

