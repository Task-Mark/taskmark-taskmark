---
id: T-146
type: task
title: Sort task list by id, title, and size
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-099, T-130]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-048
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
updated: 2026-07-29T06:48:27.505Z
started_at: 2026-07-27T05:20:06Z
completed_at: 2026-07-27T05:22:17Z
actual_ms: 0
---

# T-146: Sort task list by id, title, and size

## Description

Wire the Overall task/bug table to shared sort for **id**, **title**, and **size**.

## Acceptance criteria

- [x] Task list headers for ID, Title, and Size are sortable.
- [x] Asc/desc reorder correctly for tasks and bugs in the same list.
- [x] Changing sort resets to page 1 and keeps search/filters applied.

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
| 1 | Marco Mendão | 2026-07-27T05:20:06Z | 2026-07-27T05:20:06Z | — | Task list sort by id/title/size; shared-batch: 0 of 2min by points |
