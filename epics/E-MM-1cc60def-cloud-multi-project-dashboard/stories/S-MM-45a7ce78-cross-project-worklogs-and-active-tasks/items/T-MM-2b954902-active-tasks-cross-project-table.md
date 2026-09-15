---
id: T-MM-2b954902
type: task
title: Active tasks table across projects
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
tags: [cloud, frontend, tasks]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-2b954902: Active tasks table across projects

## Description

Sortable table of the `activeItems` from every selected project (`in_progress` and `blocked` tasks/bugs/stories): title, type and status via `StatusBadge`, priority, points, assignee avatars, project, and last update. Sorting by priority, project, and updated; rows link to the owning project board.

## Acceptance criteria

- [ ] Every `in_progress` and `blocked` item across the selected projects is listed with status badge, priority, points, assignees, and project.
- [ ] Columns sort by priority, project, and last update; the default sort puts blocked and high-priority work on top.
- [ ] Rows link to the owning project board and the table honours the global filters.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — sortable cross-project active tasks table. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
