---
id: T-067
type: task
title: Aggregate all work items into flat rows
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [similar:list-ui]
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-026
epic: E-006
owner: ""
blocked: false
cancelled: false
tags: [data, frontend, views, all]
created: 2026-07-22
updated: 2026-07-23T06:26:02.701Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-067: Aggregate all work items into flat rows

## Description

Build a data helper that flattens every epic, story, and task/bug on the active board into a single row model (id, type, title, status, points, timing, parents).

## Acceptance criteria

- [ ] Rows include all epics, stories, and tasks/bugs for the active project board.
- [ ] Each row exposes type and enough parent ids/titles for display and navigation.
- [ ] Empty board yields an empty list (no crash).

## Notes



## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-22T00:29:24Z | prompt | Create E-006 new work item list views with stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

