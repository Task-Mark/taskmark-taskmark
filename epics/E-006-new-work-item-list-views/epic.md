---
id: E-006
type: epic
title: New work item list views
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 40
points_source: rolled_up
estimate_minutes: 560
actual_minutes: 486
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, views, lists]
created: 2026-07-22
updated: 2026-07-23T09:36:52.298Z
started_at: 2026-07-23T05:44:00Z
completed_at: 2026-07-23T06:42:22Z
actual_ms: 29185000
---
# E-006: New work item list views

## Goal

Let users switch the board between Overall (current drill-down), All (flat mixed table), Stories (stories with epic tags), and Tasks (tasks with epic and story tags) via a button-group control.

## Scope

- A view switcher control (button group / segmented control) for Overall, All, Stories, and Tasks.
- Overall: preserve the current epic → story → task nested view as the default.
- All: one table with every epic, story, and task/bug.
- Stories: stories only, each with a UI tag for its parent epic.
- Tasks: tasks/bugs only, each with UI tags for parent epic and story.
- Open existing work item detail sheets from the new list rows.

## Out of scope

- Editing or creating items from the new views.
- Filtering, sorting, or saved custom views beyond the four modes.
- Changing Taskmark markdown frontmatter `tags` fields (view tags are UI parent badges).
- Cross-project aggregation beyond the active board.

## Success metrics

- User can switch among the four views with one control.
- Overall remains the default and matches today’s drill-down.
- All / Stories / Tasks show the correct row sets with the specified parent tags.
- Detail sheets still open from list rows in every view.

## Stories

- [S-024: Board list view switcher](stories/S-024-board-list-view-switcher/story.md)
- [S-025: Overall list view (current drill-down)](stories/S-025-overall-list-view/story.md)
- [S-026: All work items table view](stories/S-026-all-work-items-table-view/story.md)
- [S-027: Stories list view with epic tag](stories/S-027-stories-list-view-with-epic-tag/story.md)
- [S-028: Tasks list view with epic and story tags](stories/S-028-tasks-list-view-with-parent-tags/story.md)

## Tasks

- [x] [T-082](items/T-082-overall-and-work-items-tabs.md) — Overall and Work items tabs only
- [x] [T-084](items/T-084-work-items-created-solved-dates.md) — Show created and solved dates on work items list
- [x] [T-085](items/T-085-date-tooltips-id-done-badge.md) — Date tooltips on ID and done badge instead of columns

- [T-080: Add task and bug totals on epic and story lists](items/T-080-task-bug-totals-on-lists.md)

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| c809639 | taskmark-frontend | 2026-07-22T00:35:27Z | add tabs and update button styles |
| 603c59c | taskmark-taskmark | 2026-07-22T00:35:27Z | add e-006 list views board |
| 97685ee | taskmark-frontend | 2026-07-23T07:08:21Z | add overall and work items views |
| ce68818 | taskmark-taskmark | 2026-07-23T07:08:22Z | complete e-006 work items tabs |

## Tasks

- [x] [T-080](items/T-080-task-bug-totals-on-lists.md) — Add task and bug totals on epic and story lists
- [x] [T-081](items/T-081-work-item-totals-on-lists.md) — Count work items on lists

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-23T06:38:57Z | 2026-07-23T06:42:22Z | shared-batch parent rollup (0ms; effort on child tasks) |
| 2 | agent | 2026-07-23T07:00:14Z | 2026-07-23T07:03:14Z | T-082 Overall + Work items tabs |
| 3 | agent | 2026-07-22T00:35:27Z | 2026-07-23T07:08:22Z | auto-recovered: commit span |
