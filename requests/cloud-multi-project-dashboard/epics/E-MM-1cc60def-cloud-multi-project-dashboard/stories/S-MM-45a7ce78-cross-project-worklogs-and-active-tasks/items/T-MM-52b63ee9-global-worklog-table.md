---
id: T-MM-52b63ee9
type: task
title: Global worklog table with project column
status: backlog
priority: high
size: M
points: 5
parent: S-MM-45a7ce78
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, frontend, worklog]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-52b63ee9: Global worklog table with project column

## Description

New `DashboardWorklogTable` with the columns of `WorklogPanel` plus a project column. `WorklogPanel` cannot be reused directly because it depends on `useWorkItemSheet` (per-board detail sheet), so item badges link to the owning project board instead. Reuse `ListPagination`, `typeBadgeClass`, and `formatTaskmarkDate` from `@taskmark/components`. Feed it the merged worklog rows from all selected projects, newest first.

## Acceptance criteria

- [ ] Sessions from every selected project appear newest-first with actor, item badge, project, started/ended, and summary.
- [ ] Pagination behaves like the board worklog panel; filters by author, project, and timeframe narrow the rows.
- [ ] The item badge links to the owning project board page.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — merged worklog table with project column and pagination. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
