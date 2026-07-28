---
id: T-094
type: task
title: Paginate work items list
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-082, T-091]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-032
epic: E-009
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
tags: [dashboard, frontend, pagination, workitems]
created: 2026-07-23
updated: 2026-07-28T07:41:00.094Z
started_at: 2026-07-23T15:35:42Z
completed_at: 2026-07-23T15:41:41Z
actual_ms: 47000
---
# T-094: Paginate work items list

## Description

Wire shared pagination into the Work items tab list (stories + epic-direct tasks/bugs), preserving existing sort order before slicing.

## Acceptance criteria

- [x] Work items rows are sliced by page / pageSize after existing sort.
- [x] Shared pagination control is shown with the list.
- [x] Detail open still works for paginated rows.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T15:35:42Z | prompt | Marco Mendão | Implement epic E-009 list pagination |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T15:35:42Z | 2026-07-23T15:36:29Z | shared-batch: 47891 of 359182ms by points; delivered T-094 |
