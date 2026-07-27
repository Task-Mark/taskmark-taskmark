---
id: S-048
type: story
title: Sort Overall drill-down lists
status: done
priority: medium
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 6
points_source: rolled_up
estimate_minutes: 90
actual_minutes: 0
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
updated: 2026-07-27T07:23:21.914Z
started_at: 2026-07-27T05:20:06Z
completed_at: 2026-07-27T05:22:17Z
actual_ms: 0
---

# S-048: Sort Overall drill-down lists

## User story

As a user, I want to sort the Overall epic, story, and task tables by id, title, and size (where shown), so I can reorder drill-down lists quickly.

## Acceptance criteria

- [x] Epic list sorts by **id** and **title** (asc/desc) via column headers.
- [x] Story list sorts by **id**, **title**, and **size**.
- [x] Task list sorts by **id**, **title**, and **size**.
- [x] Sort applies after search/filters; changing sort resets pagination to page 1.

## Tasks

- [T-144: Sort epic list by id and title](items/T-144-sort-epic-list.md)
- [T-145: Sort story list by id, title, and size](items/T-145-sort-story-list.md)
- [T-146: Sort task list by id, title, and size](items/T-146-sort-task-list.md)

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
