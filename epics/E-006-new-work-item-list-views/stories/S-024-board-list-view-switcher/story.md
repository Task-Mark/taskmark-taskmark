---
id: S-024
type: story
title: Board list view switcher
status: backlog
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 6
points_source: rolled_up
estimate_minutes: 90
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-006
epic: E-006
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, views, switcher]
created: 2026-07-22
updated: 2026-07-22T00:35:34.300Z
started_at: null
completed_at: null
actual_ms: 0
---

# S-024: Board list view switcher

## User story

As a user, I want a control to switch board list views so I can pick Overall, All, Stories, or Tasks without leaving the board.

## Acceptance criteria

- [ ] A button-group (or equivalent) lists Overall, All, Stories, and Tasks.
- [ ] Selecting an option updates the active view mode and primary list region.
- [ ] The active option is visually indicated.
- [ ] Default selection is Overall.

## Tasks

- [T-062: Define list view mode types and state](items/T-062-define-list-view-mode-state.md)
- [T-063: Build view switcher button group UI](items/T-063-build-view-switcher-button-group.md)
- [T-064: Wire switcher into board shell](items/T-064-wire-switcher-into-board-shell.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-22T00:29:24Z | prompt | Create E-006 new work item list views with stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| c809639 | taskmark-frontend | 2026-07-22T00:35:27Z | add tabs and update button styles |
| 603c59c | taskmark-taskmark | 2026-07-22T00:35:27Z | add e-006 list views board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

