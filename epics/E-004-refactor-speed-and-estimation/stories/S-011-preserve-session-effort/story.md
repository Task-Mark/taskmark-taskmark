---
id: S-011
type: story
title: Preserve session effort tracking
status: backlog
priority: high
size: S
size_source: suggested
size_basis: [T-030, T-031]
points: 3
points_source: suggested
estimate_minutes: 136
actual_minutes: 0
estimate_basis: [T-030, T-031]
session_cap_minutes: 480
parent: E-004
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
# S-011: Preserve session effort tracking

## User story

As a team using Taskmark, I want AI/human session elapsed time still stored so we keep effort history even as actual meaning changes.

## Acceptance criteria

- [ ] Work log sessions continue to record Started/Ended and billable elapsed minutes.
- [ ] Session effort is retained as a first-class signal (documented field name, e.g. effort_minutes or work-log-derived).
- [ ] Conventions clarify effort (sessions) vs actual (start→complete).

## Tasks

- [T-030: Document effort vs actual dual model](items/T-030-document-effort-vs-actual.md)
- [T-031: Keep work-log session effort computation](items/T-031-keep-work-log-effort.md)

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

