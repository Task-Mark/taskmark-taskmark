---
id: T-031
type: task
title: Keep work-log session effort computation
status: done
priority: high
size: M
size_source: suggested
size_basis: [calibrated:T-031]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 4
estimate_basis: [calibrated:T-031]
session_cap_minutes: 480
parent: S-011
epic: E-004
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
tags: [effort, work-log, conventions]
created: 2026-07-21
updated: 2026-07-24T16:49:37.998Z
started_at: 2026-07-21T22:35:27Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 240000
---

# T-031: Keep work-log session effort computation

## Description

Ensure recompute still derives session effort from Work log (idle/session caps) and stores it without dropping history.

## Acceptance criteria

- [x] Work-log billable minutes still computed on sync/complete.
- [x] Existing session rows remain valid.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T22:56:48Z | prompt | Marco Mendão | Create epic: refactor speed/estimation — 1-month velocity, start/end cascade, dual effort vs actual |
| 2 | 2026-07-21T23:07:27Z | feedback | Marco Mendão | E-004 dual model delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T22:35:27Z | 2026-07-21T22:39:27Z | auto-backfilled: velocity × points (missing work log); shared-batch: 4 of 7min by points |

