---
id: S-013
type: story
title: Estimate from rolling speed
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 6
points_source: rolled_up
estimate_minutes: 100
actual_minutes: 96
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-004
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [estimation, create, velocity]
created: 2026-07-21
updated: 2026-07-23T04:38:56.857Z
started_at: 2026-07-21T21:31:27Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 5760000
---

# S-013: Estimate from rolling speed

## User story

As someone creating a task, I want estimate_minutes suggested from recent speed × points so plans match how fast we currently deliver.

## Acceptance criteria

- [x] create-task/story/epic suggest estimate_minutes = points × 1-month min/point when sample size is sufficient.
- [x] Falls back to SIZING seed table when window is insufficient.
- [x] estimate_basis records the velocity source (window median vs seed).

## Tasks

- [T-035: Suggest estimates from monthly velocity on create](items/T-035-suggest-estimate-from-velocity.md)
- [T-036: Optionally refresh open estimates when velocity updates](items/T-036-recalibrate-open-estimates.md)

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
| 1 | agent | 2026-07-21T21:31:27Z | 2026-07-21T23:07:27Z | auto-backfilled: velocity × points (missing work log) |

