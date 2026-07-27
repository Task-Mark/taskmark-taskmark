---
id: S-012
type: story
title: One-month velocity window
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 8
points_source: rolled_up
estimate_minutes: 85
actual_minutes: 112
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-004
epic: E-004
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [velocity, estimation]
created: 2026-07-21
updated: 2026-07-27T07:36:40.469Z
started_at: 2026-07-21T21:15:27Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 6720000
---
# S-012: One-month velocity window

## User story

As a planner, I want minutes-per-point computed from done work in the last month so speed reflects recent delivery, not all-time noise.

## Acceptance criteria

- [x] Velocity samples done tasks/bugs (and documented story/epic rollups if used) with completed_at in the last 30 days.
- [x] Primary speed metric is median (or documented aggregate) actual-or-effort minutes per point for that window.
- [x] VELOCITY.md reports the 1-month window and sample counts; insufficient data falls back clearly.

## Tasks

- [T-032: Define 1-month done-item sample set](items/T-032-define-month-window-samples.md)
- [T-033: Compute minutes per point for window](items/T-033-compute-minutes-per-point.md)
- [T-034: Refresh VELOCITY.md for monthly window](items/T-034-refresh-velocity-md-month.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T22:56:48Z | prompt | Marco Mendão | Create epic: refactor speed/estimation — 1-month velocity, start/end cascade, dual effort vs actual |
| 2 | 2026-07-21T23:07:27Z | feedback | Marco Mendão | E-004 dual model delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T21:15:27Z | 2026-07-21T23:07:27Z | auto-backfilled: velocity × points (missing work log) |

