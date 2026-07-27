---
id: T-091
type: task
title: Paginate epic list
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-006, T-089]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-031
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
tags: [dashboard, frontend, pagination, epics]
created: 2026-07-23
updated: 2026-07-27T05:18:44.416Z
started_at: 2026-07-23T15:35:42Z
completed_at: 2026-07-23T15:41:41Z
actual_ms: 47000
---
# T-091: Paginate epic list

## Description

Wire the shared pagination control into the Overall epic list so only the current page of epics is shown.

## Acceptance criteria

- [x] Epic table rows are sliced by page / pageSize.
- [x] Pagination control is rendered with the epic list.
- [x] Selecting an epic on the current page still updates drill-down as today.

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
| 1 | Marco Mendão | 2026-07-23T15:35:42Z | 2026-07-23T15:36:29Z | shared-batch: 47891 of 359182ms by points; delivered T-091 |
