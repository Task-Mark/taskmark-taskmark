---
id: S-031
type: story
title: Paginate Overall drill-down lists
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 6
points_source: rolled_up
estimate_minutes: 90
actual_minutes: 2
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-009
epic: E-009
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
tags: [dashboard, frontend, pagination, overall]
created: 2026-07-23
updated: 2026-07-24T16:57:53.518Z
started_at: 2026-07-23T15:35:42Z
completed_at: 2026-07-23T15:41:41Z
actual_ms: 141000
---

# S-031: Paginate Overall drill-down lists

## User story

As a user viewing Overall, I want epic, story, and task tables paginated with the shared control, so long boards are easy to browse without losing drill-down behavior.

## Acceptance criteria

- [x] Epic list shows only the current page of epics and the pagination control.
- [x] Story list (for selected epic) is paginated the same way.
- [x] Task list (for selected story) is paginated the same way.
- [x] Selecting a different epic/story resets that child list to page 1.
- [x] Detail open / row selection still works on paginated rows.

## Tasks

- [T-091: Paginate epic list](items/T-091-paginate-epic-list.md)
- [T-092: Paginate story list](items/T-092-paginate-story-list.md)
- [T-093: Paginate task list](items/T-093-paginate-task-list.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T15:29:50Z | prompt | Marco Mendão | Create epic for list pagination with nav + page size; include stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T15:35:42Z | 2026-07-23T15:35:42Z | shared-batch parent rollup (0 min); leaves hold effort |
