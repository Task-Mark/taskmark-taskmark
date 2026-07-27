---
id: T-173
type: task
title: Implement 90-day weekly points average
status: backlog
priority: high
size: L
size_source: suggested
size_basis: [T-033, T-032]
points: 5
points_source: suggested
estimate_minutes: 70
actual_minutes: 0
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
resolvers: []
blocked: false
cancelled: false
tags: [frontend, metrics, velocity]
created: 2026-07-27
updated: 2026-07-27T06:17:22.249Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-173: Implement 90-day weekly points average

## Description

Implement Current Speed: start from the ISO week of the latest completed task/bug, walk back 90 days, sum story points completed per week, then average those weekly sums. Prefer leaf tasks/bugs with `points` and `completed_at`.

## Acceptance criteria

- [ ] Anchor week = week containing max `completed_at` among done tasks/bugs.
- [ ] Window covers ~90 days ending at that week (include all weeks that intersect the window).
- [ ] Weekly total = sum of `points` for items completed in that week.
- [ ] Speed = mean of weekly totals; weeks with no completions count as `0`.
- [ ] No completed leaves → return `null` / empty so UI can show `—`.
- [ ] Pure helper with clear unit-testable week bucketing (UTC or local — pick one, document).

## Notes

This dashboard metric is independent of `VELOCITY.md`’s 30-day minutes-per-point window.

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
