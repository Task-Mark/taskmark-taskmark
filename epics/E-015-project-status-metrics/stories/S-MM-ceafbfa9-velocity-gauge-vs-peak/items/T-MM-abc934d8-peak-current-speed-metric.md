---
id: T-MM-abc934d8
type: task
title: Compute peak historical Current Speed
status: done
priority: medium
size: M
points: 5
parent: S-MM-ceafbfa9
epic: E-015
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
tags: [frontend, metrics, velocity]
created: 2026-08-30
updated: 2026-08-30T07:06:06Z
started_at: 2026-08-30T06:57:15Z
completed_at: 2026-08-30T07:06:06Z
---

# T-MM-abc934d8: Compute peak historical Current Speed

Keep the existing Current Speed rule (90-day weekly average of done task/bug points, skip the current ISO week and zero-point weeks). Extract an as-of helper so the same average can be evaluated at week ends. Add a peak over every ISO week from the first completion through now, and expose `peakSpeedPtsPerWeek` plus `peakSpeedWeekLabel` on `ProjectStatusMetrics`. Static snapshots inherit the fields via `computeProjectStatusMetrics`.

## Acceptance criteria

- [x] `computeCurrentSpeedPtsPerWeek` still matches today’s average when called with `now`.
- [x] Peak is the maximum of that average at each considered week, including `now`, so peak is never below current.
- [x] `ProjectStatusMetrics` includes `peakSpeedPtsPerWeek` and `peakSpeedWeekLabel` (null when there is no speed).
- [x] Unit tests cover peak above current, peak equal to current, no completions, and zero-point weeks ignored.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-30T06:51:01Z | prompt | Marco Mendão | Cursor plan: velocity gauge whose max is historical peak Current Speed (90-day weekly average), shown as a Bklit arc gauge in the metrics strip with #C4A1FF retro styling. |
| 2026-08-30T06:57:15Z | prompt | Marco Mendão | /tkmd-do S-MM-ceafbfa9 e S-MM-0ae91e44 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-30T06:57:15Z | 2026-08-30T07:06:06Z | Peak Current Speed as-of week ends; expose peak fields on metrics |
