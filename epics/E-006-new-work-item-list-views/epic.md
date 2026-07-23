---
id: E-006
type: epic
title: New work item list views
status: backlog
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 30
points_source: rolled_up
estimate_minutes: 435
actual_minutes: 0
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
updated: 2026-07-23T05:10:21.353Z
started_at: null
completed_at: null
actual_ms: 0
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

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| c809639 | taskmark-frontend | 2026-07-22T00:35:27Z | add tabs and update button styles |
| 603c59c | taskmark-taskmark | 2026-07-22T00:35:27Z | add e-006 list views board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

