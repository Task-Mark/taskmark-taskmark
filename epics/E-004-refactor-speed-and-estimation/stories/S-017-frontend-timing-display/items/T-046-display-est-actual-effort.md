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
estimate_minutes: 120
actual_minutes: 0
estimate_basis: []
session_cap_minutes: 480
parent: S-017
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [frontend, estimation, actual]
created: 2026-07-21
updated: 2026-07-21T23:18:07Z
started_at: 2026-07-21T23:00:19Z
completed_at: 2026-07-21T23:01:18Z
---
# T-046: Display Est Actual and optional Effort in lists

## Description

Epic/story/task tables keep Est and Actual; show Effort when any row has effort_minutes.

## Acceptance criteria

- [x] Est and Actual columns remain on all three lists.
- [x] Effort column appears when effort data exists.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T23:00:19Z | prompt | Ensure frontend keeps showing estimate and actual after latest Taskmark changes |
| 2 | 2026-07-21T23:01:18Z | feedback | timing display delivered |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| 9e136f1 | taskmark-frontend | 2026-07-21T23:02:38Z | harden est actual timing display for flat boards |
| 0806511 | taskmark-taskmark | 2026-07-21T23:02:38Z | add S-017 frontend timing display and sync board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T23:00:19Z | 2026-07-21T23:01:18Z | Frontend timing display hardened for flat boards |
