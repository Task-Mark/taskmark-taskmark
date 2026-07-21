---
id: T-031
type: task
title: Keep work-log session effort computation
status: backlog
priority: high
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 120
actual_minutes: 0
estimate_basis: []
session_cap_minutes: 480
parent: S-011
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [effort, work-log, conventions]
created: 2026-07-21
updated: 2026-07-21T23:01:27Z
started_at: null
completed_at: null
---
# T-031: Keep work-log session effort computation

## Description

Ensure recompute still derives session effort from Work log (idle/session caps) and stores it without dropping history.

## Acceptance criteria

- [ ] Work-log billable minutes still computed on sync/complete.
- [ ] Existing session rows remain valid.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T22:56:48Z | prompt | Create epic: refactor speed/estimation — 1-month velocity, start/end cascade, dual effort vs actual |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

