---
id: S-024
type: story
title: Board list view switcher
status: done
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
tags: [dashboard, frontend, views, switcher]
created: 2026-07-22
updated: 2026-07-29T11:30:07.936Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:42:22Z
actual_ms: 39000
---

# S-024: Board list view switcher

## User story

As a user, I want a control to switch board list views so I can pick Overall, All, Stories, or Tasks without leaving the board.

## Acceptance criteria

- [x] A button-group (or equivalent) lists Overall, All, Stories, and Tasks.
- [x] Selecting an option updates the active view mode and primary list region.
- [x] The active option is visually indicated.
- [x] Default selection is Overall.

## Tasks

- [T-062: Define list view mode types and state](items/T-062-define-list-view-mode-state.md)
- [T-063: Build view switcher button group UI](items/T-063-build-view-switcher-button-group.md)
- [T-064: Wire switcher into board shell](items/T-064-wire-switcher-into-board-shell.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-22T00:29:24Z | prompt | Marco Mendão | Create E-006 new work item list views with stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| c809639 | taskmark-frontend | 2026-07-22T00:35:27Z | Marco Mendão | add tabs and update button styles |
| 603c59c | taskmark-taskmark | 2026-07-22T00:35:27Z | Marco Mendão | add e-006 list views board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T06:38:57Z | 2026-07-23T06:38:57Z | shared-batch parent rollup (0ms; effort on child tasks) |
