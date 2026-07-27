---
id: T-046
type: task
title: Display Est Actual and optional Effort in lists
status: done
priority: high
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 2
estimate_basis: [calibrated:T-046]
session_cap_minutes: 480
parent: S-017
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
tags: [frontend, estimation, actual]
created: 2026-07-21
updated: 2026-07-27T05:16:43.229Z
started_at: 2026-07-21T23:00:19Z
completed_at: 2026-07-21T23:01:18Z
actual_ms: 120000
---
# T-046: Display Est Actual and optional Effort in lists

## Description

Epic/story/task tables keep Est and Actual; show Effort when any row has effort_minutes.

## Acceptance criteria

- [x] Est and Actual columns remain on all three lists.
- [x] Effort column appears when effort data exists.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T23:00:19Z | prompt | Marco Mendão | Ensure frontend keeps showing estimate and actual after latest Taskmark changes |
| 2 | 2026-07-21T23:01:18Z | feedback | Marco Mendão | timing display delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 9e136f1 | taskmark-frontend | 2026-07-21T23:02:38Z | Marco Mendão | harden est actual timing display for flat boards |
| 0806511 | taskmark-taskmark | 2026-07-21T23:02:38Z | Marco Mendão | add S-017 frontend timing display and sync board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T22:29:18Z | 2026-07-21T22:31:18Z | auto-backfilled: velocity × points (missing work log); shared-batch: 2 of 4min by points |
