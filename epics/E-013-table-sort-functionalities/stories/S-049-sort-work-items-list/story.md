---
id: S-049
type: story
title: Sort Work items list
status: done
priority: medium
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 70
actual_minutes: 1
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-013
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
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-27T05:20:06Z
completed_at: 2026-07-27T05:22:17Z
actual_ms: 60000
---
# S-049: Sort Work items list

## User story

As a user, I want to sort the Work items table by epic, size, title, and id, so I can scan and compare items across the board.

## Acceptance criteria

- [x] Work items table sorts by **id**, **title**, **size**, and **epic** (asc/desc).
- [x] Epic sort uses a stable key (epic id or title) with missing-epic rows ordered consistently.
- [x] Sort composes with search, parent/tag/hide-completed, and timeframe filters; changing sort resets to page 1.

## Tasks

- [T-147: Sort work items by id, title, size, and epic](items/T-147-sort-work-items-list.md)
- [T-148: Compose sort with filters and pagination](items/T-148-compose-sort-filters-pagination.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:19:23Z | prompt | Marco Mendão | Create stories and tasks for E-013 table sort (epic, size, title, id) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 4b6097c | taskmark-frontend | 2026-07-27T06:34:38+01:00 | Marco Mendão | add sortable table columns across board lists |
| f14af32 | taskmark-taskmark | 2026-07-27T06:34:38+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T05:20:06Z | 2026-07-27T05:20:06Z | — | Rollup: children hold shared-batch for E-013 |
