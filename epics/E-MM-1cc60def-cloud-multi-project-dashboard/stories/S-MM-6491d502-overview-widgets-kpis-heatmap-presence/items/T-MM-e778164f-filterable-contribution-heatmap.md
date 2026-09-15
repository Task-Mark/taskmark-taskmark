---
id: T-MM-e778164f
type: task
title: Contribution heatmap filterable by author and project
status: backlog
priority: high
size: M
points: 5
parent: S-MM-6491d502
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, frontend, heatmap]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-e778164f: Contribution heatmap filterable by author and project

## Description

Reuse `PointsHeatmap` from `@taskmark/components` for the aggregated contribution calendar. The enriched completion samples from the API carry `resolvers`, so filtering by author and project happens before samples enter the component, which only needs `completedAt` and `points`. Merge samples across the selected projects into one calendar.

## Acceptance criteria

- [ ] The heatmap shows points completed per day across all selected projects.
- [ ] Narrowing by author recolours the calendar using only that author's completions; project and timeframe filters combine with it.
- [ ] Day tooltips keep the existing points label format from the board heatmap.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — contribution heatmap with author/project filtering via enriched completion samples. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
