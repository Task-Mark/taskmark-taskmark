---
id: S-013
type: story
title: Estimate from rolling speed
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-035, T-036]
points: 6
points_source: suggested
estimate_minutes: 960
actual_minutes: 0
estimate_basis: [T-035, T-036]
session_cap_minutes: 480
parent: E-004
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [estimation, create, velocity]
created: 2026-07-21
updated: 2026-07-21T23:01:27Z
started_at: null
completed_at: null
---
# S-013: Estimate from rolling speed

## User story

As someone creating a task, I want estimate_minutes suggested from recent speed × points so plans match how fast we currently deliver.

## Acceptance criteria

- [ ] create-task/story/epic suggest estimate_minutes = points × 1-month min/point when sample size is sufficient.
- [ ] Falls back to SIZING seed table when window is insufficient.
- [ ] estimate_basis records the velocity source (window median vs seed).

## Tasks

- [T-035: Suggest estimates from monthly velocity on create](items/T-035-suggest-estimate-from-velocity.md)
- [T-036: Optionally refresh open estimates when velocity updates](items/T-036-recalibrate-open-estimates.md)

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

