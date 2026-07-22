---
id: S-014
type: story
title: Actual time from start to complete
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 8
points_source: rolled_up
estimate_minutes: 130
actual_minutes: 128
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-004
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [actual, started_at, completed_at]
created: 2026-07-21
updated: 2026-07-22T00:16:21.562Z
started_at: 2026-07-21T20:59:27Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 7680000
---
# S-014: Actual time from start to complete

## User story

As a reviewer of delivery, I want actual_minutes to reflect time from when work started to when it completed so lead time is visible alongside session effort.

## Acceptance criteria

- [x] For done items with started_at and completed_at, actual_minutes = elapsed between those timestamps (documented caps if applied).
- [x] recompute-actuals writes this actual and rolls up parents per new rules.
- [x] Completing without started_at or without a usable start date follows an explicit policy (prompt user, derive from first work-log session, or leave null — documented and implemented).

## Tasks

- [T-037: Define wall-clock actual_minutes rules](items/T-037-define-wall-clock-actual.md)
- [T-038: Update recompute for start→complete actuals](items/T-038-recompute-wall-clock-actuals.md)
- [T-039: Handle complete without start or missing dates](items/T-039-handle-missing-start.md)

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
| 1 | agent | 2026-07-21T20:59:27Z | 2026-07-21T23:07:27Z | auto-backfilled: velocity × points (missing work log) |

