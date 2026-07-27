---
id: S-028
type: story
title: Tasks list view with epic and story tags
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 7
points_source: rolled_up
estimate_minutes: 110
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-006
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
tags: [dashboard, frontend, views, tasks]
created: 2026-07-22
updated: 2026-07-27T07:45:28.202Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:42:22Z
actual_ms: 46000
---
# S-028: Tasks list view with epic and story tags

## User story

As a user, I want a Tasks view that lists only tasks with tags for their epic and story so I can browse leaf work across the board.

## Acceptance criteria

- [x] Tasks view lists only tasks and bugs.
- [x] Each row shows tags/badges for parent epic and parent story.
- [x] Activating a row opens the task/bug detail sheet.
- [x] Empty state is handled when there are no tasks.

## Tasks

- [T-073: Collect tasks with epic and story metadata](items/T-073-collect-tasks-with-parent-metadata.md)
- [T-074: Build Tasks view table with epic and story tags](items/T-074-build-tasks-view-with-parent-tags.md)
- [T-075: Wire Tasks view into switcher and detail sheet](items/T-075-wire-tasks-view-to-switcher.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-22T00:29:24Z | prompt | Marco Mendão | Create E-006 new work item list views with stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T06:38:57Z | 2026-07-23T06:38:57Z | shared-batch parent rollup (0ms; effort on child tasks) |
