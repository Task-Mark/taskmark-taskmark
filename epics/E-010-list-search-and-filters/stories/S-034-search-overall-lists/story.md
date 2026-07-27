---
id: S-034
type: story
title: Search on Overall drill-down lists
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 6
points_source: rolled_up
estimate_minutes: 90
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-010
epic: E-010
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
tags: [dashboard, frontend, search, overall]
created: 2026-07-23
updated: 2026-07-27T07:45:28.202Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-23T16:03:09Z
actual_ms: 36000
---

# S-034: Search on Overall drill-down lists

## User story

As a user on Overall, I want to search epics, stories, and tasks by code or title, so I can jump to the right row without scrolling.

## Acceptance criteria

- [x] Epic list has a search box filtering by epic id/title.
- [x] Story list has a search box filtering by story id/title.
- [x] Task list has a search box filtering by task/bug id/title.
- [x] Search composes with pagination (page resets to 1 when the query changes).

## Tasks

- [T-097: Search epic list](items/T-097-search-epic-list.md)
- [T-098: Search story list](items/T-098-search-story-list.md)
- [T-099: Search task list](items/T-099-search-task-list.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T15:53:02Z | prompt | Marco Mendão | Epic for list search + parent/tag filters + hide completed; create stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:00:49Z | rollup: children hold shared-batch; delivered S-034 |
