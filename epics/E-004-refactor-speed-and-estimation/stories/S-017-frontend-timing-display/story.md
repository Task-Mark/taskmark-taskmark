---
id: S-017
type: story
title: Frontend timing display for estimate and actual
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 7
points_source: rolled_up
estimate_minutes: 106
actual_minutes: 80
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-004
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
tags: [frontend, estimation, actual, effort]
created: 2026-07-21
updated: 2026-07-25T10:24:50.747Z
started_at: 2026-07-21T23:00:19Z
completed_at: 2026-07-21T23:01:18Z
actual_ms: 4800000
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
- [T-061: Show precise Actual with seconds or milliseconds](items/T-061-precise-actual-display.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T23:00:19Z | prompt | Marco Mendão | Ensure frontend keeps showing estimate and actual after latest Taskmark changes |
| 2 | 2026-07-21T23:01:18Z | feedback | Marco Mendão | timing display delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| ff5d088 | taskmark-frontend | 2026-07-22T00:17:56Z | Marco Mendão | show precise actual duration |
| 0b6df50 | taskmark-taskmark | 2026-07-22T00:17:57Z | Marco Mendão | sync taskmark board |
| 9e136f1 | taskmark-frontend | 2026-07-21T23:02:38Z | Marco Mendão | harden est actual timing display for flat boards |
| 0806511 | taskmark-taskmark | 2026-07-21T23:02:38Z | Marco Mendão | add S-017 frontend timing display and sync board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T21:41:18Z | 2026-07-21T23:01:18Z | auto-backfilled: velocity × points (missing work log) |
