---
id: S-017
type: story
title: Frontend timing display for estimate and actual
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-045, T-046, T-047]
points: 5
points_source: suggested
estimate_minutes: 256
actual_minutes: 0
estimate_basis: [T-045, T-046, T-047]
session_cap_minutes: 480
parent: E-004
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [frontend, estimation, actual, effort]
created: 2026-07-21
updated: 2026-07-21T23:02:48Z
started_at: 2026-07-21T23:00:19Z
completed_at: 2026-07-21T23:01:18Z
---
# S-017: Frontend timing display for estimate and actual

## User story

As a dashboard user, I want estimate and actual minutes to keep showing correctly for flat multi-repo boards (and effort when present) so timing stays visible after the Taskmark layout and speed-model changes.

## Acceptance criteria

- [x] Epic, story, and task lists still show Est and Actual from `estimate_minutes` / `actual_minutes`.
- [x] Parsers work with flat `*-taskmark` board roots (not only nested `taskmark/`).
- [x] Optional `effort_minutes` is parsed; Effort column shows when any row has it.
- [x] Verified against the live `taskmark-taskmark` board (E-004 values visible).

## Tasks

- [T-045: Shared frontmatter timing field helpers](items/T-045-shared-timing-helpers.md)
- [T-046: Display Est Actual and optional Effort in lists](items/T-046-display-est-actual-effort.md)
- [T-047: Verify timing parse against flat board](items/T-047-verify-flat-board-timing.md)

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
