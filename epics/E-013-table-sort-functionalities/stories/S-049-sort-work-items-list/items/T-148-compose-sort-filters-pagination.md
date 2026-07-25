---
id: T-148
type: task
title: Compose sort with filters and pagination
status: backlog
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
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, lists, sort]
created: 2026-07-24
updated: 2026-07-25T10:44:19.816Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-148: Compose sort with filters and pagination

## Description

Ensure sort state composes cleanly with search, parent/tag/hide-completed, timeframe, and pagination across lists that support sort.

## Acceptance criteria

- [ ] Sort runs on the already-filtered set (does not clear filters).
- [ ] Changing sort (key or direction) resets pagination to page 1 on Overall and Work items lists.
- [ ] Clearing filters or timeframe does not wipe the active sort unless intentionally reset.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:19:23Z | prompt | Marco Mendão | Create stories and tasks for E-013 table sort (epic, size, title, id) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
