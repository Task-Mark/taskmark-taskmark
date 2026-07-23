---
id: T-079
type: task
title: Show General epic with unattached items in UI
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-006, T-012]
points: 3
points_source: suggested
estimate_minutes: 45
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-029
epic: E-007
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, hierarchy]
created: 2026-07-23
updated: 2026-07-23T04:38:56.857Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-079: Show General epic with unattached items in UI

## Description

Ensure the dashboard epic list always surfaces the **General** epic and that its stories/tasks (unattached work) are browsable like any other epic, including safe handling of missing parent metadata in list/detail views.

## Acceptance criteria

- [ ] Epic list includes General when present on the board.
- [ ] Selecting General shows its stories and tasks (unattached work).
- [ ] Stories/Tasks/All views tolerate null or General-only parents without blank/crash rows.
- [ ] Empty General (no children yet) still appears and has a clear empty state.

## Notes



## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-23T04:38:20Z | prompt | Allow standalone stories/tasks; infer parents from context; default General epic for unattached work |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
