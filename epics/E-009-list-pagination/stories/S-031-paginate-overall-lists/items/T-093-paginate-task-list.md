---
id: T-093
type: task
title: Paginate task list
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-015, T-092]
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
blocked: false
cancelled: false
tags: [dashboard, frontend, pagination, tasks]
created: 2026-07-23
updated: 2026-07-23T16:24:32.159Z
started_at: 2026-07-23T15:35:42Z
completed_at: 2026-07-23T15:41:41Z
actual_ms: 47000
---
# T-093: Paginate task list

## Description

Wire shared pagination into the Overall task/bug list for the selected story.

## Acceptance criteria

- [x] Task table rows are sliced by page / pageSize.
- [x] Changing the selected story resets task list to page 1.
- [x] Detail open still works for paginated rows.

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-23T15:35:42Z | prompt | Implement epic E-009 list pagination |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-23T15:35:42Z | 2026-07-23T15:36:29Z | shared-batch: 47891 of 359182ms by points; delivered T-093 |
