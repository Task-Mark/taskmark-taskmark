---
id: E-004
type: epic
title: Refactor speed and estimation
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 52
points_source: rolled_up
estimate_minutes: 682
actual_minutes: 688
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
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
tags: [velocity, estimation, effort, plugin, conventions]
created: 2026-07-21
updated: 2026-07-28T07:41:00.094Z
started_at: 2026-07-21T23:05:18Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 41280000
estimate_source: rolled_up
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

- [S-023: Shared batch actual time split](stories/S-023-shared-batch-actual-split/story.md)

- [S-011: Preserve session effort tracking](stories/S-011-preserve-session-effort/story.md)
- [S-012: One-month velocity window](stories/S-012-one-month-velocity-window/story.md)
- [S-013: Estimate from rolling speed](stories/S-013-estimate-from-rolling-speed/story.md)
- [S-014: Actual time from start to complete](stories/S-014-actual-from-start-complete/story.md)
- [S-015: Start cascade for task, story, epic](stories/S-015-start-cascade/story.md)
- [S-016: End cascade for task, story, epic](stories/S-016-end-cascade/story.md)
- [S-017: Frontend timing display for estimate and actual](stories/S-017-frontend-timing-display/story.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 79848e9 | taskmark-cursor | 2026-07-22T00:17:56Z | Marco Mendão | fix shared batch actual split |
| ff5d088 | taskmark-frontend | 2026-07-22T00:17:56Z | Marco Mendão | show precise actual duration |
| 0b6df50 | taskmark-taskmark | 2026-07-22T00:17:57Z | Marco Mendão | sync taskmark board |
| 82bf126 | taskmark-cursor | 2026-07-21T23:27:54Z | Marco Mendão | require work logs on complete for accurate actuals |
| 6204471 | taskmark-taskmark | 2026-07-21T23:27:54Z | Marco Mendão | backfill work logs on done items from velocity |
| 6aca5e6 | taskmark-cursor | 2026-07-21T23:20:34Z | Marco Mendão | update speed estimation and epic points rollup |
| 123ecb7 | taskmark-frontend | 2026-07-21T23:20:34Z | Marco Mendão | show est actual only and drop epic size |
| 9883b62 | taskmark-taskmark | 2026-07-21T23:20:34Z | Marco Mendão | sync e-004 timing and points rollup on board |
| 9e136f1 | taskmark-frontend | 2026-07-21T23:02:38Z | Marco Mendão | harden est actual timing display for flat boards |
| 0806511 | taskmark-taskmark | 2026-07-21T23:02:38Z | Marco Mendão | add S-017 frontend timing display and sync board |
| 758cd8c | taskmark-taskmark | 2026-07-21T22:58:00Z | Marco Mendão | add e-004 speed and estimation epic |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T11:39:27Z | 2026-07-21T15:07:27Z | auto-backfilled: velocity × points (missing work log) |
| 2 | Marco Mendão | 2026-07-21T15:07:27Z | 2026-07-21T23:07:27Z | auto-backfilled: velocity × points (missing work log) |
