---
id: S-048
type: story
title: Sort Overall drill-down lists
status: backlog
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
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, lists, sort]
created: 2026-07-24
updated: 2026-07-27T05:16:43.229Z
started_at: null
completed_at: null
actual_ms: 0
---
# S-048: Sort Overall drill-down lists

## User story

As a user, I want to sort the Overall epic, story, and task tables by id, title, and size (where shown), so I can reorder drill-down lists quickly.

## Acceptance criteria

- [ ] Epic list sorts by **id** and **title** (asc/desc) via column headers.
- [ ] Story list sorts by **id**, **title**, and **size**.
- [ ] Task list sorts by **id**, **title**, and **size**.
- [ ] Sort applies after search/filters; changing sort resets pagination to page 1.

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

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
