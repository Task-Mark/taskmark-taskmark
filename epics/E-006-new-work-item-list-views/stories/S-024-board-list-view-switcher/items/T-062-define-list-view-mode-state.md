---
id: T-062
type: task
title: Define list view mode types and state
status: backlog
priority: high
size: S
size_source: suggested
size_basis: [similar:list-ui]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-024
epic: E-006
owner: ""
blocked: false
cancelled: false
tags: [state, frontend, views]
created: 2026-07-22
updated: 2026-07-23T06:26:02.701Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-062: Define list view mode types and state

## Description

Introduce a shared list-view mode model (Overall, All, Stories, Tasks) and controlled state for the active mode in the board UI.

## Acceptance criteria

- [ ] A typed view-mode union covers Overall, All, Stories, and Tasks.
- [ ] Board UI can hold and update the active view mode in shared state.
- [ ] Default active mode is Overall.

## Notes

Reuse existing board layout state patterns; do not build the switcher UI here.

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-22T00:29:24Z | prompt | Create E-006 new work item list views with stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

