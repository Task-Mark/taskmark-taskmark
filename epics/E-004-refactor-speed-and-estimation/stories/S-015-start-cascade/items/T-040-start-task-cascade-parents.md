---
id: T-040
type: task
title: Start task cascades to story and epic
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_basis: [calibrated:T-040]
session_cap_minutes: 480
parent: S-015
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
tags: [start-work, cascade, status]
created: 2026-07-21
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-21T22:19:27Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 0
---
# T-040: Start task cascades to story and epic

## Description

Extend start-work so starting a leaf sets parent started_at timestamps.

## Acceptance criteria

- [x] Task start sets parents' started_at when null.
- [x] Status becomes in_progress appropriately.

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

