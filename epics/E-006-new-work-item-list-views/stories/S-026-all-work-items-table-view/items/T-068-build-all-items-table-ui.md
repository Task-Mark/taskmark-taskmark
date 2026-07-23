---
id: T-068
type: task
title: Build All view unified table UI
status: done
priority: high
size: M
size_source: suggested
size_basis: [similar:list-ui]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-026
epic: E-006
owner: ""
blocked: false
cancelled: false
tags: [ui, frontend, views, all]
created: 2026-07-22
updated: 2026-07-23T09:36:52.298Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:39:17Z
actual_ms: 20000
---

# T-068: Build All view unified table UI

## Description

Render the All view as one table listing every work item with clear type distinction and core columns (id, title, status, size/points, est/actual as already used elsewhere).

## Acceptance criteria

- [x] All view shows a single table of mixed-type rows.
- [x] Type is visually distinguishable (epic/story/task/bug).
- [x] Table is usable for large boards (scroll, readable density).

## Notes



## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-23T06:42:22Z | prompt | Implement E-006 |
| 2 | 2026-07-23T06:42:22Z | feedback | Shipped list view as part of E-006 |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-23T06:38:57Z | 2026-07-23T06:39:17Z | shared-batch: 20500 of 205000ms by points |
