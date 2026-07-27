---
id: T-173
type: task
title: Implement 90-day weekly points average
status: done
priority: high
size: L
size_source: suggested
size_basis: [T-033, T-032]
points: 5
points_source: suggested
estimate_minutes: 70
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-055
epic: E-015
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
tags: [frontend, metrics, velocity]
created: 2026-07-27
updated: 2026-07-27T07:23:21.914Z
started_at: 2026-07-27T06:25:20Z
completed_at: 2026-07-27T06:28:48Z
actual_ms: 60000
---

# T-173: Implement 90-day weekly points average

## Description

Implement Current Speed: start from the latest completed task/bug, walk back 90 days, sum story points completed per ISO week, then average **only weeks with points > 0**, excluding the **current** ISO week.

## Acceptance criteria

- [x] Anchor = max `completed_at` among done tasks/bugs; window looks back 90 days.
- [x] Weekly total = sum of `points` for tasks/bugs completed in that ISO week.
- [x] Exclude the current ISO week from the average.
- [x] Exclude weeks with 0 points from numerator and denominator.
- [x] Speed = mean of remaining weekly totals; no considered weeks → `null` / `—`.
- [x] Pure helper with ISO week bucketing.

## Notes

Idle/hold weeks (0 pts) and the in-progress current week are ignored so speed reflects active delivery weeks only.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T05:55:45Z | prompt | Marco Mendão | Create epic for project status metrics (total/complete/speed + contributors) styled like neo-brutalism metric cards; include stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:26:20Z | 2026-07-27T06:27:20Z | shared-batch: 1 of 3min by points — implement E-015 (T-173) |
