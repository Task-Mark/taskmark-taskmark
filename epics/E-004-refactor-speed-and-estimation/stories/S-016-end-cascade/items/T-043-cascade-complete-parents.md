---
id: T-043
type: task
title: Cascade complete parents when last child ends
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_basis: [calibrated:T-043]
session_cap_minutes: 480
parent: S-016
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [complete-work, cascade, status]
created: 2026-07-21
updated: 2026-07-23T09:47:44.562Z
started_at: 2026-07-21T22:19:27Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 0
---

# T-043: Cascade complete parents when last child ends

## Description

After leaf complete, auto-complete story/epic when children satisfy done rules.

## Acceptance criteria

- [x] Last task complete closes story.
- [x] Last story complete closes epic.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T22:56:48Z | prompt | Create epic: refactor speed/estimation — 1-month velocity, start/end cascade, dual effort vs actual |
| 2 | 2026-07-21T23:07:27Z | feedback | E-004 dual model delivered |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T22:19:27Z | 2026-07-21T22:19:27Z | auto-backfilled: velocity × points (missing work log); shared-batch: 0 of 1min by points |

