---
id: S-011
type: story
title: Preserve session effort tracking
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 4
points_source: rolled_up
estimate_minutes: 21
actual_minutes: 20
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
tags: [effort, work-log, conventions]
created: 2026-07-21
updated: 2026-07-28T07:27:54.696Z
started_at: 2026-07-21T23:05:18Z
completed_at: 2026-07-21T23:07:27Z
actual_ms: 1200000
---

# S-011: Preserve session effort tracking

## User story

As a team using Taskmark, I want AI/human session elapsed time still stored so we keep effort history even as actual meaning changes.

## Acceptance criteria

- [x] Work log sessions continue to record Started/Ended and billable elapsed minutes.
- [x] Session effort is retained as a first-class signal (documented field name, e.g. effort_minutes or work-log-derived).
- [x] Conventions clarify effort (sessions) vs actual (start→complete).

## Tasks

- [T-030: Document effort vs actual dual model](items/T-030-document-effort-vs-actual.md)
- [T-031: Keep work-log session effort computation](items/T-031-keep-work-log-effort.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T23:05:18Z | prompt | Marco Mendão | develop the epic E-004 |
| 1 | 2026-07-21T22:56:48Z | prompt | Marco Mendão | Create epic: refactor speed/estimation — 1-month velocity, start/end cascade, dual effort vs actual |
| 2 | 2026-07-21T23:07:27Z | feedback | Marco Mendão | E-004 dual model delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 6aca5e6 | taskmark-cursor | 2026-07-21T23:20:34Z | Marco Mendão | update speed estimation and epic points rollup |
| 123ecb7 | taskmark-frontend | 2026-07-21T23:20:34Z | Marco Mendão | show est actual only and drop epic size |
| 9883b62 | taskmark-taskmark | 2026-07-21T23:20:34Z | Marco Mendão | sync e-004 timing and points rollup on board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T22:19:27Z | 2026-07-21T22:19:27Z | auto-backfilled: velocity × points (missing work log); shared-batch: 0min rollup (children hold allocation) |
| 2 | Marco Mendão | 2026-07-21T23:05:18Z | 2026-07-21T23:20:34Z | auto-recovered: commit span |

