---
id: T-177
type: task
title: Remove velocity docs and VELOCITY.md
status: done
priority: high
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 2
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-057
epic: E-015
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
tags: [plugin, velocity, shelved]
created: 2026-07-27
updated: 2026-07-28T07:41:00.094Z
started_at: 2026-07-27T06:10:41Z
completed_at: 2026-07-27T06:17:22Z
actual_ms: 120000
---
# T-177: Remove velocity docs and VELOCITY.md

## Description

Delete velocity command/skill/docs/sample and board `VELOCITY.md`; update init/folder layout.

## Acceptance criteria

- [x] Board `VELOCITY.md` opens with a shelved notice (keep last metrics below for reference).
- [x] Plugin convention + command docs say shelved / do not use for estimates.
- [x] No deletion of historical throughput tables.


## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T06:10:25Z | prompt | Marco Mendão | Shelf velocity docs and estimate mechanism for now; reimplement later |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| a494e58 | taskmark-taskmark | 2026-07-27T06:19:46Z | Marco Mendão | add e-015 metrics and remove velocity board |
| 1a8522f | taskmark-frontend | 2026-07-27T06:19:45Z | Marco Mendão | drop est actual columns and velocity timing notes |
| b942bb0 | taskmark-cursor | 2026-07-27T06:19:45Z | Marco Mendão | remove velocity and time-estimate sizing |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:10:41Z | 2026-07-27T06:12:41Z | shared-batch: 2 of 6min by points — remove velocity (T-177) |
