---
id: S-026
type: story
title: All work items table view
status: done
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 10
points_source: rolled_up
estimate_minutes: 160
actual_minutes: 5
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
tags: [dashboard, frontend, views, all]
created: 2026-07-22
updated: 2026-07-25T10:44:19.816Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:42:22Z
actual_ms: 313000
---
# S-026: All work items table view

## User story

As a user, I want an All view that puts every epic, story, and task on one table so I can scan the whole board at once.

## Acceptance criteria

- [x] All view shows one table with every epic, story, and task/bug on the active board.
- [x] Row type is visually clear.
- [x] Activating a row opens the existing detail sheet for that item.
- [x] Empty boards show an empty state without errors.

## Tasks

- [T-067: Aggregate all work items into flat rows](items/T-067-aggregate-all-work-item-rows.md)
- [T-068: Build All view unified table UI](items/T-068-build-all-items-table-ui.md)
- [T-069: Wire All view into switcher and detail sheet](items/T-069-wire-all-view-to-switcher.md)
- [T-108: Sort done work items by completed date](items/T-108-sort-done-by-completed-date.md)
- [T-109: Done work items sort by solved date only](items/T-109-done-sort-by-solved-not-priority.md)

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
