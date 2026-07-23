---
id: E-005
type: epic
title: View work item
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 32
points_source: rolled_up
estimate_minutes: 510
actual_minutes: 3
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, detail, sheet]
created: 2026-07-21
updated: 2026-07-23T06:26:02.701Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 195000
---

# E-005: View work item

## Goal

Let users open any work item (epic, user story, or task) in a dedicated view mode that presents every available detail in the clearest layout, always inside a sheet.

## Scope

- View mode for epics, user stories, and tasks (bugs use the same item view as tasks where applicable).
- Present all work-item information in the best layout for each type (frontmatter fields, goal/user story/description, acceptance criteria, children, work log, commits, prompt & feedback, timing, and related metadata).
- Every work-item view is presented in a sheet (slide-over / drawer), not a full-page route replacement.
- Open the sheet from existing list UIs (epic, story, and task lists) without breaking the current drill-down hierarchy.
- Empty and error states when a selected item cannot be loaded or has sparse content.

## Out of scope

- Editing or creating work items from the sheet.
- Separate full-page detail routes.
- Cross-project detail views (scoped to the active project board).
- Reordering or bulk actions from the sheet.

## Success metrics

- From any epic, story, or task list row, the user can open that item’s detail view in a sheet.
- The sheet shows the item’s details clearly and appropriately for its type.
- Closing the sheet returns the user to the same list/drill-down context.

## Stories

- [S-018: Work item detail sheet](stories/S-018-work-item-detail-sheet/story.md)
- [S-019: Load full work item content](stories/S-019-load-full-work-item-content/story.md)
- [S-020: Epic detail view](stories/S-020-epic-detail-view/story.md)
- [S-021: Story detail view](stories/S-021-story-detail-view/story.md)
- [S-022: Task and bug detail view](stories/S-022-task-detail-view/story.md)

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| e890d82 | taskmark-taskmark | 2026-07-21T23:52:01Z | add e-005 view work item board |
| 5756d6a | taskmark-frontend | 2026-07-22T00:00:33Z | add work item detail sheet |
| cedb561 | taskmark-taskmark | 2026-07-22T00:00:33Z | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T23:53:57Z | 2026-07-21T23:53:57Z | Delivered as part of E-005; shared-batch: 0ms rollup (children hold allocation) |
| 1 | agent | 2026-07-21T23:53:57Z | 2026-07-21T23:56:38Z | Implemented work item detail sheets (S-018–S-022) |
