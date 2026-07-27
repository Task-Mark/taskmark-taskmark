---
id: S-057
type: story
title: Remove legacy velocity and time estimates
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 7
points_source: rolled_up
estimate_minutes: 100
actual_minutes: 6
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-015
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
tags: [plugin, velocity, estimation, shelved]
created: 2026-07-27
updated: 2026-07-27T06:20:07Z
started_at: 2026-07-27T06:10:41Z
completed_at: 2026-07-27T06:17:22Z
actual_ms: 360000
---

# S-057: Shelf legacy velocity estimation

## User story

As a Taskmark maintainer, I want the old velocity/time-estimate mechanism removed from the plugin, so sizing only suggests t-shirt size and story points (no minutes-from-velocity or seed time estimates).

## Acceptance criteria

- [x] `VELOCITY.md`, `/velocity`, and `taskmark-velocity` removed from plugin and board.
- [x] `recompute-actuals` no longer computes median min/point, refreshes velocity, or calibrates/suggests time estimates.
- [x] Create/sizing skills suggest **size + points only**; `estimate_minutes` defaults to `0`.
- [x] Docs/rules/init no longer require or refresh velocity.
- [x] Local plugin install synced.

## Tasks

- [T-177: Mark velocity docs as shelved](items/T-177-mark-velocity-docs-shelved.md)
- [T-178: Disable velocity-based estimate refresh](items/T-178-disable-velocity-estimate-refresh.md)
- [T-179: Update create and velocity skills for seeds-only](items/T-179-skills-seeds-only-while-shelved.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T06:10:25Z | prompt | Marco Mendão | Shelf velocity docs and estimate mechanism for now; reimplement later |
| 2 | 2026-07-27T06:14:14Z | prompt | Marco Mendão | Clarify: shelf = remove velocity/time-estimate from code; sizing only suggests size + points |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| a494e58 | taskmark-taskmark | 2026-07-27T06:19:46Z | Marco Mendão | add e-015 metrics and remove velocity board |
| 1a8522f | taskmark-frontend | 2026-07-27T06:19:45Z | Marco Mendão | drop est actual columns and velocity timing notes |
| b942bb0 | taskmark-cursor | 2026-07-27T06:19:45Z | Marco Mendão | remove velocity and time-estimate sizing |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:10:41Z | 2026-07-27T06:10:41Z | Parent rollup: velocity removed; billable on T-177–T-179 (shared-batch) |
