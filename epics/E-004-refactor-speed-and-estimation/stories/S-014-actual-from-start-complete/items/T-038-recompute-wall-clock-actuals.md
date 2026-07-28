---
id: T-038
type: task
title: Update recompute for start→complete actuals
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_basis: [calibrated:T-038]
session_cap_minutes: 480
parent: S-014
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
tags: [actual, started_at, completed_at]
created: 2026-07-21
updated: 2026-07-28T09:08:49.505Z
started_at: 2026-07-21T22:19:27Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 0
---

# T-038: Update recompute for start→complete actuals

## Description

Change recompute-actuals.py to set leaf actual from started_at/completed_at and roll up parents.

## Acceptance criteria

- [x] Script implements new actual.
- [x] INDEX/VELOCITY use new values.

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
| 1 | Marco Mendão | 2026-07-21T22:19:27Z | 2026-07-21T22:19:27Z | auto-backfilled: velocity × points (missing work log); shared-batch: 0 of 1min by points |

