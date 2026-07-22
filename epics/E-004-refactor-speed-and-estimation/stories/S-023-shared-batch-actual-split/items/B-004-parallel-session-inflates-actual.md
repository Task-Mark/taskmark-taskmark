---
id: B-004
type: bug
title: Parallel full-session work logs inflate epic Actual
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-038, T-031]
points: 5
points_source: suggested
estimate_minutes: 80
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-023
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [actual, work-log, batch, bug]
created: 2026-07-22
updated: 2026-07-22T00:16:21.562Z
started_at: 2026-07-22T00:07:36Z
completed_at: 2026-07-22T00:09:05Z
actual_ms: 89000
---

# B-004: Parallel full-session work logs inflate epic Actual

## Description

When an agent implements an entire epic in one sitting, it often writes the same Work log Started/Ended (e.g. 10 minutes) on every task. Parent Actual = sum of children, so a 10-minute epic becomes N×10 on the story/epic and corrupts velocity.

## Repro steps

1. Create an epic with multiple stories and tasks.
2. Ask the AI to implement the whole epic in one session (~10 minutes wall clock).
3. Observe each task Work log uses the full ~10 minute span.
4. Story/epic Actual becomes roughly tasks × 10 instead of ~10.

## Fix criteria

- [x] Document shared-batch allocation: one wall-clock span; split minutes across leaves by points; parents roll up the sum.
- [x] Update complete-work / start-work / work-log / effort-time accordingly.
- [x] recompute-actuals redistributes identical (Started, Ended) leaf sessions under an epic proportional to points.
- [x] After recompute, E-005 epic Actual equals the single batch span (not 13×).

## Notes

Weight = story points (fallback estimate_minutes). Use largest-remainder so allocated minutes sum exactly to batch billable.

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-22T00:07:36Z | prompt | Bug: implementing an epic copies full session onto every task and inflates Actual |
| 2 | 2026-07-22T00:09:05Z | feedback | Shared-batch Actual fix delivered; E-005 Actual now equals batch span |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-22T00:07:36Z | 2026-07-22T00:09:05Z | Fixed shared-batch Actual split (recompute + conventions) |
