---
id: S-023
type: story
title: Shared batch actual time split
status: done
priority: high
size: S
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 80
actual_minutes: 1
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-004
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [actual, work-log, batch, velocity]
created: 2026-07-22
updated: 2026-07-22T00:18:29.117Z
started_at: 2026-07-22T00:07:36Z
completed_at: 2026-07-22T00:09:05Z
actual_ms: 89000
---

# S-023: Shared batch actual time split

## User story

As a user who asks the AI to implement a whole epic in one session, I want Actual minutes on the epic to equal the wall-clock time spent, with that time divided across tasks by effort, so story/epic rollups stay honest.

## Acceptance criteria

- [x] Conventions and complete-work forbid copying the full batch Started/Ended onto every leaf.
- [x] Batch delivery allocates billable minutes to leaves proportional to points (largest-remainder), summing to the batch total.
- [x] recompute-actuals detects identical sibling batch sessions and redistributes; parent Actual equals the batch total (not N× batch).
- [x] E-005 inflated Actuals are corrected by redistribution.

## Tasks

- [B-004: Parallel full-session work logs inflate epic Actual](items/B-004-parallel-session-inflates-actual.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-22T00:07:36Z | prompt | Bug: implementing an epic copies full session onto every task and inflates Actual |
| 2 | 2026-07-22T00:09:05Z | feedback | Shared-batch Actual fix delivered |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| 79848e9 | taskmark-cursor | 2026-07-22T00:17:56Z | fix shared batch actual split |
| 0b6df50 | taskmark-taskmark | 2026-07-22T00:17:57Z | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-22T00:07:36Z | 2026-07-22T00:07:36Z | shared-batch: 0min rollup (children hold allocation) |
