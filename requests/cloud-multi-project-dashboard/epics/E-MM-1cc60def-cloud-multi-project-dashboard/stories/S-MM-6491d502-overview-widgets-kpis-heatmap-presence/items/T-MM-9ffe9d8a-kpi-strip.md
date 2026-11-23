---
id: T-MM-9ffe9d8a
type: task
title: Dashboard KPI strip
status: backlog
priority: high
size: S
points: 3
parent: S-MM-6491d502
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, frontend, metrics]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-9ffe9d8a: Dashboard KPI strip

## Description

KPI strip using `MetricStatCard` from `@taskmark/components`: count of active projects, tasks currently in progress across projects, points completed this ISO week (sum of `currentWeekPointsDone`), worklog sessions inside the filtered period, and distinct active contributors. Values recompute from the filtered data.

## Acceptance criteria

- [ ] Five KPI cards render from the aggregated payload and honour the global filters.
- [ ] Numbers match the underlying filtered widgets (e.g., sessions equals the worklog table row count for the same filters).
- [ ] The strip collapses gracefully on mobile widths.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — KPI strip with cross-project headline metrics. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
