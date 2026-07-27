---
id: T-147
type: task
title: Sort work items by id, title, size, and epic
status: done
priority: medium
size: M
size_source: suggested
size_basis: [T-100, T-131]
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
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
updated: 2026-07-27T06:17:22.249Z
started_at: 2026-07-27T05:20:06Z
completed_at: 2026-07-27T05:22:17Z
actual_ms: 60000
---
# T-147: Sort work items by id, title, size, and epic

## Description

Wire the Work items table to shared sort for **id**, **title**, **size**, and **epic**.

## Acceptance criteria

- [x] Work items headers for ID, Title, Size, and Epic are sortable.
- [x] Epic sort uses a stable key (epic title with id tie-break, or epic id) and places missing-epic rows consistently.
- [x] Asc/desc reorder the filtered result set correctly.

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
| 1 | Marco Mendão | 2026-07-27T05:20:06Z | 2026-07-27T05:21:06Z | — | Work items sort by id/title/size/epic; shared-batch: 1 of 2min by points |
