---
id: T-079
type: task
title: Show General epic with unattached items in UI
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-006, T-012]
points: 3
points_source: suggested
estimate_minutes: 45
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-029
epic: E-007
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
tags: [dashboard, frontend, hierarchy]
created: 2026-07-23
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-23T04:44:50Z
completed_at: 2026-07-23T04:45:50Z
actual_ms: 60000
---
# T-079: Show General epic with unattached items in UI

## Description

Ensure the dashboard epic list always surfaces the **General** epic and that its stories/tasks (unattached work) are browsable like any other epic, including safe handling of missing parent metadata in list/detail views.

## Acceptance criteria

- [x] Epic list includes General when present on the board.
- [x] Selecting General shows its stories and tasks (unattached work).
- [x] Stories/Tasks/All views tolerate null or General-only parents without blank/crash rows.
- [x] Empty General (no children yet) still appears and has a clear empty state.

## Notes



## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T04:38:20Z | prompt | Marco Mendão | Allow standalone stories/tasks; infer parents from context; default General epic for unattached work |
| 2 | 2026-07-23T04:45:32Z | prompt | Marco Mendão | Develop S-029 |
| 3 | 2026-07-23T04:45:32Z | feedback | Marco Mendão | Done as part of S-029 shared batch |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T04:44:50Z | 2026-07-23T04:45:50Z | shared-batch: 1 of 4min by points; delivered T-079 |
