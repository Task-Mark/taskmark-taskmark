---
id: T-148
type: task
title: Compose sort with filters and pagination
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-104, T-132]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-049
epic: E-013
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
tags: [dashboard, frontend, lists, sort]
created: 2026-07-24
updated: 2026-07-27T05:37:38.663Z
started_at: 2026-07-27T05:20:06Z
completed_at: 2026-07-27T05:22:17Z
actual_ms: 0
---

# T-148: Compose sort with filters and pagination

## Description

Ensure sort state composes cleanly with search, parent/tag/hide-completed, timeframe, and pagination across lists that support sort.

## Acceptance criteria

- [x] Sort runs on the already-filtered set (does not clear filters).
- [x] Changing sort (key or direction) resets pagination to page 1 on Overall and Work items lists.
- [x] Clearing filters or timeframe does not wipe the active sort unless intentionally reset.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:19:23Z | prompt | Marco Mendão | Create stories and tasks for E-013 table sort (epic, size, title, id) |
| 99 | 2026-07-27T05:22:17Z | prompt | Marco Mendão | Implement this E-013 |
| 100 | 2026-07-27T05:22:17Z | feedback | Marco Mendão | Delivered as part of E-013 shared batch |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 4b6097c | taskmark-frontend | 2026-07-27T06:34:38+01:00 | Marco Mendão | add sortable table columns across board lists |
| f14af32 | taskmark-taskmark | 2026-07-27T06:34:38+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T05:20:06Z | 2026-07-27T05:20:06Z | — | Compose sort with filters and pagination; shared-batch: 0 of 2min by points |
