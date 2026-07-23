---
id: T-087
type: task
title: Add date-fns and format all displayed dates
status: done
priority: medium
size: XS
size_source: suggested
size_basis: [calibrated:T-087]
points: 1
points_source: suggested
estimate_minutes: 25
actual_minutes: 23
estimate_source: suggested
estimate_basis: [calibrated:T-087]
session_cap_minutes: 480
parent: E-005
epic: E-005
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, dates, detail]
created: 2026-07-23
updated: 2026-07-23T16:33:36.080Z
started_at: 2026-07-23T09:44:14Z
completed_at: 2026-07-23T09:47:31Z
actual_ms: 1436000
---

# T-087: Add date-fns and format all displayed dates

## Description

Add `date-fns` and use it to format every user-visible date/time in the dashboard (detail meta, tooltips, commits, work log, prompt tables) instead of raw ISO / frontmatter strings.

## Acceptance criteria

- [x] `date-fns` is a project dependency.
- [x] Shared helpers format Taskmark date-only and datetime strings.
- [x] Detail sheet Created / Updated / Started / Completed use formatted dates.
- [x] Commits, work log, and prompt table date columns are formatted.
- [x] Created / Solved tooltips use the same formatting.

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-23T09:44:14Z | prompt | Add date-fns and format all dates |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| ea40442 | taskmark-frontend | 2026-07-23T10:04:53Z | format dates with date-fns |
| bbab1eb | taskmark-taskmark | 2026-07-23T10:04:53Z | add t-087 date-fns board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-23T09:44:14Z | 2026-07-23T09:47:31Z | date-fns helpers; format detail + tooltip dates |
| 2 | agent | 2026-07-23T09:44:14Z | 2026-07-23T10:04:53Z | auto-recovered: commit span |
