---
id: E-013
type: epic
title: Table sort functionalities
status: done
priority: medium
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 21
points_source: rolled_up
estimate_minutes: 305
actual_minutes: 2
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
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
updated: 2026-08-17T08:03:41.619Z
started_at: 2026-07-27T05:20:06Z
completed_at: 2026-07-27T05:26:10Z
actual_ms: 120000
---

# E-013: Table sort functionalities

## Goal

Let users sort work-item tables by epic, size, title, and id so they can quickly reorder lists to find and compare items.

## Scope

- Sortable columns (or equivalent controls) for: **epic**, **size**, **title**, and **id**.
- Apply across board list tables where those columns appear (Overall drill-down and Work items / list views as applicable).
- Ascending and descending toggle; clear visual indicator of active sort column and direction.
- Compose with existing search, filters, timeframe, and pagination (reset page on sort change when needed).

## Out of scope

- Multi-column / secondary sort keys.
- Persisting sort in the URL or user preferences (optional later).
- Server-side sort APIs.

## Success metrics

- User can sort any supported table by epic, size, title, or id in either direction.
- Active sort is obvious; clearing or switching columns behaves predictably with filters and pagination.

## Stories

- [S-047: Shared table sort plumbing](stories/S-047-shared-table-sort-plumbing/story.md)
- [S-048: Sort Overall drill-down lists](stories/S-048-sort-overall-lists/story.md)
- [S-049: Sort Work items list](stories/S-049-sort-work-items-list/story.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 4b6097c | taskmark-frontend | 2026-07-27T06:34:38+01:00 | Marco Mendão | add sortable table columns across board lists |
| f14af32 | taskmark-taskmark | 2026-07-27T06:34:38+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T05:20:06Z | 2026-07-27T05:20:06Z | Rollup: children hold shared-batch (2min) |
