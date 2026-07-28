---
id: T-066
type: task
title: Preserve drill-down under Overall view
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
parent: S-025
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
tags: [frontend, views, overall]
created: 2026-07-22
updated: 2026-07-28T14:32:06.722Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:39:10Z
actual_ms: 13000
---
# T-066: Preserve drill-down under Overall view

## Description

Keep epic list → story list → task list selection behavior unchanged when Overall is active; other modes must not break Overall.

## Acceptance criteria

- [x] Epic, story, and task selection/drill-down work as before in Overall.
- [x] Switching away from Overall and back restores Overall drill-down without losing project context.
- [x] Work item detail sheet still opens from Overall list rows.

## Notes



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
