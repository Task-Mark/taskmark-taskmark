---
id: E-009
type: epic
title: Work items list view
status: backlog
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 21
points_source: rolled_up
estimate_minutes: 330
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, views, workitems]
created: 2026-07-23
updated: 2026-07-23T06:36:20Z
started_at: null
completed_at: null
actual_ms: 0
---

# E-009: Work items list view

## Goal

Give users a **Work items** board tab that lists every user story, task, and bug on the project in one place, ordered by status then priority, with epic/priority badges and story drill-down into that story’s tasks and bugs.

## Scope

- New **Work items** tab on the board view switcher.
- Flat list of all stories, tasks, and bugs for the active project (not epics).
- Primary sort: status (`backlog` → `in_progress` → `done`); secondary sort: priority.
- Epic badge shows epic **id** only; hover tooltip shows epic **title**.
- Priority badge on each row.
- Clicking a **story** row shows that story’s task/bug list.

## Out of scope

- Listing epics in this tab (see E-006 All view for mixed epic+story+task tables).
- Replacing Overall drill-down as the default view.
- Editing items inline from the Work items list.

## Success metrics

- Users can scan all leaf and story work without opening every epic.
- Status/priority ordering matches the agreed order.
- Story click lands on the correct task/bug list.

## Stories

- [S-030: Work items tab in board switcher](stories/S-030-work-items-tab/story.md)
- [S-031: Collect and sort work items](stories/S-031-collect-and-sort-work-items/story.md)
- [S-032: Work items list with epic and priority badges](stories/S-032-work-items-list-badges/story.md)
- [S-033: Story click shows task and bug list](stories/S-033-story-click-task-list/story.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| 6201583 | taskmark-taskmark | 2026-07-23T06:36:19Z | add e-009 work items list view epic |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

