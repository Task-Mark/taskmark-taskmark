---
id: E-004
type: epic
title: Refactor speed and estimation
status: backlog
priority: high
size: XL
size_source: suggested
size_basis: [S-011, S-012, S-013, S-014, S-015, S-016, S-017]
points: 43
points_source: suggested
estimate_minutes: 5192
actual_minutes: 0
estimate_basis: [S-011, S-012, S-013, S-014, S-015, S-016, S-017]
session_cap_minutes: 480
parent: null
epic: null
owner: ""
blocked: false
cancelled: false
tags: [velocity, estimation, effort, plugin, conventions]
created: 2026-07-21
updated: 2026-07-21T23:02:48Z
started_at: null
completed_at: null
---
# E-004: Refactor speed and estimation

## Goal

Refactor how Taskmark measures speed and estimates work: keep AI/human **session effort**, compute **minutes-per-point over a 1-month window**, estimate from that speed, redefine **actual** as wall-clock from start→complete, and add explicit **start/end** actions with parent/child cascade.

## Scope

- Continue recording elapsed session time (work log) as effort spent by AI/human.
- Calculate story-point speed from done tasks/stories/epics in a rolling **1-month** window.
- Derive new-item `estimate_minutes` from that speed × points.
- Recalculate `actual_minutes` from `started_at` → `completed_at` (not calendar idle alone without a start).
- Handle complete-without-start / missing dates explicitly.
- Start action for task/story/epic; starting a task also starts its story and epic if needed.
- End/complete action; ending the last open child closes the parent story/epic.

## Out of scope

- Changing Fibonacci points map or t-shirt labels.
- Dashboard UI charts (plugin/board model first; UI can follow).
- Billing/invoicing integrations.

## Success metrics

- New estimates use 1-month median min/point when enough samples exist; otherwise seed table.
- Done items with both start and complete timestamps have actual = that span (with documented caps if any).
- Start/end skills cascade correctly; last child complete closes parents.
- Session work-log effort remains available (not discarded).

## Stories

- [S-011: Preserve session effort tracking](stories/S-011-preserve-session-effort/story.md)
- [S-012: One-month velocity window](stories/S-012-one-month-velocity-window/story.md)
- [S-013: Estimate from rolling speed](stories/S-013-estimate-from-rolling-speed/story.md)
- [S-014: Actual time from start to complete](stories/S-014-actual-from-start-complete/story.md)
- [S-015: Start cascade for task, story, epic](stories/S-015-start-cascade/story.md)
- [S-016: End cascade for task, story, epic](stories/S-016-end-cascade/story.md)
- [S-017: Frontend timing display for estimate and actual](stories/S-017-frontend-timing-display/story.md)

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| 9e136f1 | taskmark-frontend | 2026-07-21T23:02:38Z | harden est actual timing display for flat boards |
| 0806511 | taskmark-taskmark | 2026-07-21T23:02:38Z | add S-017 frontend timing display and sync board |
| 758cd8c | taskmark-taskmark | 2026-07-21T22:58:00Z | add e-004 speed and estimation epic |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
