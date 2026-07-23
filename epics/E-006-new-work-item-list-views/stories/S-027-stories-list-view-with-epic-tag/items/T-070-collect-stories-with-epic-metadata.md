---
id: T-070
type: task
title: Collect stories with epic metadata
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
parent: S-027
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
tags: [data, frontend, views, stories]
created: 2026-07-22
updated: 2026-07-23T17:36:48Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:39:10Z
actual_ms: 13000
---

# T-070: Collect stories with epic metadata

## Description

Build a data helper that lists every story on the board with its parent epic id/title for tagging.

## Acceptance criteria

- [x] All stories across epics are included for the active board.
- [x] Each row includes epic id and title (or equivalent) for the tag.
- [x] Stories without a resolvable epic are handled safely (omit or show fallback).

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
