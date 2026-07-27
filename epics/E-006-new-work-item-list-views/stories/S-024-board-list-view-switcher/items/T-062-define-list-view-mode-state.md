---
id: T-062
type: task
title: Define list view mode types and state
status: done
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
tags: [state, frontend, views]
created: 2026-07-22
updated: 2026-07-27T07:45:28.202Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:39:10Z
actual_ms: 13000
---
# T-062: Define list view mode types and state

## Description

Introduce a shared list-view mode model (Overall, All, Stories, Tasks) and controlled state for the active mode in the board UI.

## Acceptance criteria

- [x] A typed view-mode union covers Overall, All, Stories, and Tasks.
- [x] Board UI can hold and update the active view mode in shared state.
- [x] Default active mode is Overall.

## Notes

Reuse existing board layout state patterns; do not build the switcher UI here.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T06:42:22Z | prompt | Marco Mendão | Implement E-006 |
| 2 | 2026-07-23T06:42:22Z | feedback | Marco Mendão | Shipped list view as part of E-006 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T06:38:57Z | 2026-07-23T06:39:10Z | shared-batch: 13667 of 205000ms by points |
