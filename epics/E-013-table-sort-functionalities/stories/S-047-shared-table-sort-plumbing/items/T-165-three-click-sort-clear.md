---
id: T-165
type: task
title: Three-click sort cycle clears to default
status: done
priority: medium
size: XS
size_source: suggested
size_basis: [T-143]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-047
epic: E-013
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
tags: [dashboard, frontend, lists, sort]
created: 2026-07-27
updated: 2026-07-28T07:41:00.094Z
started_at: 2026-07-27T05:25:37Z
completed_at: 2026-07-27T05:26:10Z
actual_ms: 0
---

# T-165: Three-click sort cycle clears to default

## Description

Sortable headers should cycle: first click starts ascending sort, second click inverts to descending, third click clears sort and restores the list’s default order.

## Acceptance criteria

- [x] First click on a column sorts ascending.
- [x] Second click on the same column sorts descending.
- [x] Third click clears sort (null state / default order).
- [x] Clicking a different column starts ascending on that column.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T05:25:37Z | prompt | Marco Mendão | Third click should reset sort to default |
| 2 | 2026-07-27T05:26:10Z | feedback | Marco Mendão | Three-click clear implemented |
| 3 | 2026-07-27T05:34:45Z | prompt | Marco Mendão | Hide sort icon until column is actively sorted |
| 4 | 2026-07-27T05:34:45Z | feedback | Marco Mendão | Inactive columns show no icon |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 4b6097c | taskmark-frontend | 2026-07-27T06:34:38+01:00 | Marco Mendão | add sortable table columns across board lists |
| f14af32 | taskmark-taskmark | 2026-07-27T06:34:38+01:00 | Marco Mendão | sync taskmark board |
| 4f7cdb0 | taskmark-frontend | 2026-07-27T06:36:43+01:00 | Marco Mendão | hide sort icon until column is active |
| 2c23d3b | taskmark-taskmark | 2026-07-27T06:36:43+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Duration | Note |
|---------|-------|---------------|-------------|----------|------|
| 1 | Marco Mendão | 2026-07-27T05:25:37Z | 2026-07-27T05:26:10Z | — | Cycle none→asc→desc→none |
