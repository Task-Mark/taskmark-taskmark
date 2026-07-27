---
id: T-067
type: task
title: Aggregate all work items into flat rows
status: done
priority: high
size: M
size_source: suggested
size_basis: [similar:list-ui]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-026
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
tags: [data, frontend, views, all]
created: 2026-07-22
updated: 2026-07-27T06:17:22.249Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:39:17Z
actual_ms: 20000
---

# T-067: Aggregate all work items into flat rows

## Description

Build a data helper that flattens every epic, story, and task/bug on the active board into a single row model (id, type, title, status, points, timing, parents).

## Acceptance criteria

- [x] Rows include all epics, stories, and tasks/bugs for the active project board.
- [x] Each row exposes type and enough parent ids/titles for display and navigation.
- [x] Empty board yields an empty list (no crash).

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
| 1 | Marco Mendão | 2026-07-23T06:38:57Z | 2026-07-23T06:39:17Z | shared-batch: 20500 of 205000ms by points |
