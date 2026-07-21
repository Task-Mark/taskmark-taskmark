---
id: S-018
type: story
title: Work item detail sheet
status: backlog
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
parent: E-005
epic: E-005
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, sheet, detail]
created: 2026-07-21
updated: 2026-07-21T23:50:12Z
started_at: null
completed_at: null
---
# S-018: Work item detail sheet

## User story

As a user, I want every work item view to open in a sheet so I can inspect details without leaving the board drill-down.

## Acceptance criteria

- [ ] A shared sheet shell hosts work item detail content (title/header, scrollable body, close control).
- [ ] Users can open the sheet from epic, story, and task list rows without breaking existing selection/drill-down.
- [ ] Closing the sheet returns to the same list context (selection preserved).
- [ ] Loading, empty, and error states are handled inside the sheet.

## Tasks

- [T-048: Build shared work item sheet shell](items/T-048-shared-work-item-sheet-shell.md)
- [T-049: Open sheet from epic story and task list rows](items/T-049-open-sheet-from-list-rows.md)
- [T-050: Sheet loading empty and error states](items/T-050-sheet-loading-empty-error-states.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T23:48:59Z | prompt | Create all user stories and tasks for E-005 view work item |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
