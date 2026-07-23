---
id: T-035
type: task
title: Suggest estimates from monthly velocity on create
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_basis: [calibrated:T-035]
session_cap_minutes: 480
parent: S-013
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [estimation, create, velocity]
created: 2026-07-21
updated: 2026-07-23T05:10:21.353Z
started_at: 2026-07-21T22:19:27Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 0
---

# T-035: Suggest estimates from monthly velocity on create

## Description

Update create-* skills/scripts to prefer monthly velocity × points.

## Acceptance criteria

- [x] Create skills use monthly speed when available.
- [x] estimate_basis documents source.

## Notes

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
| 1 | agent | 2026-07-21T22:19:27Z | 2026-07-21T22:19:27Z | auto-backfilled: velocity × points (missing work log); shared-batch: 0 of 1min by points |

