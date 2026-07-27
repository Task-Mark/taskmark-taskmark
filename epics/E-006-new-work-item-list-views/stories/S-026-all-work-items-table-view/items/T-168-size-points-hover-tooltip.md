---
id: T-168
type: task
title: Show points on size hover in work item lists
status: done
priority: low
size: XS
size_source: suggested
size_basis: [T-106]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-026
epic: E-006
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
tags: [dashboard, frontend, lists, ui]
created: 2026-07-27
updated: 2026-07-27T07:06:27.645Z
started_at: 2026-07-27T05:37:12Z
completed_at: 2026-07-27T05:37:45Z
actual_ms: 0
---

# T-168: Show points on size hover in work item lists

## Description

On Overall work items and the Work items tab, hovering the Size cell shows the story points for that row.

## Acceptance criteria

- [x] Hovering Size on Overall work items shows points (or — when missing).
- [x] Hovering Size on the Work items tab shows points the same way.
- [x] Points column removed from Overall and Work items tables (points via size hover).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T05:37:12Z | prompt | Marco Mendão | Size column should show points on hover (overall + workitems) |
| 2 | 2026-07-27T05:37:45Z | feedback | Marco Mendão | SizeWithPointsTooltip on both lists |
| 3 | 2026-07-27T05:38:41Z | prompt | Marco Mendão | Remove the points column from these tables |
| 4 | 2026-07-27T05:38:41Z | feedback | Marco Mendão | Dropped Points column; points remain on size hover |
| 5 | 2026-07-27T05:39:47Z | prompt | Marco Mendão | Status should always be the last column |
| 6 | 2026-07-27T05:39:47Z | feedback | Marco Mendão | Work items: Priority before Status |
| 7 | 2026-07-27T05:42:24Z | prompt | Marco Mendão | Status header center; status cells align right |
| 8 | 2026-07-27T05:42:24Z | feedback | Marco Mendão | Status align center header / right content on lists |
| 9 | 2026-07-27T05:44:16Z | prompt | Marco Mendão | Center-align status and priority instead |
| 10 | 2026-07-27T05:44:16Z | feedback | Marco Mendão | Status and priority header+cells centered |
| 11 | 2026-07-27T05:45:36Z | prompt | Marco Mendão | Remove actual and estimation columns |
| 12 | 2026-07-27T05:45:36Z | feedback | Marco Mendão | Dropped Est and Actual from overall + work items |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 9328f72 | taskmark-frontend | 2026-07-27T06:45:22+01:00 | Marco Mendão | polish work item columns size tooltip and alignment |
| aa19198 | taskmark-taskmark | 2026-07-27T06:45:23+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Duration | Note |
|---------|-------|---------------|-------------|----------|------|
| 1 | Marco Mendão | 2026-07-27T05:37:12Z | 2026-07-27T05:37:45Z | — | Size tooltip with points |
