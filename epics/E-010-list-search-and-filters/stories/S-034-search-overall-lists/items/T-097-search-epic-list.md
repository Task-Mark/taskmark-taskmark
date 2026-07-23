---
id: T-097
type: task
title: Search epic list
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-091, T-096]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-034
epic: E-010
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, search, epics]
created: 2026-07-23
updated: 2026-07-23T16:16:14.881Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-23T16:03:09Z
actual_ms: 12000
---
# T-097: Search epic list

## Description

Wire the shared search box into the Overall epic list; filter before pagination.

## Acceptance criteria

- [x] Search box visible on epic list cards.
- [x] Rows filtered by epic id/title via shared helper.
- [x] Page resets to 1 when the query changes.

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-23T16:03:09Z | prompt | implement E-010 list search and filters |
| 2 | 2026-07-23T16:03:09Z | feedback | delivered search, parent/tags filters, hide completed |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-23T16:00:49Z | 2026-07-23T16:01:01Z | shared-batch: 12792 of 140714ms by points; delivered T-097 |
