---
id: S-047
type: story
title: Shared table sort plumbing
status: done
priority: medium
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 10
points_source: rolled_up
estimate_minutes: 145
actual_minutes: 1
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-013
epic: E-013
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
tags: [dashboard, frontend, lists, sort]
created: 2026-07-24
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-27T05:20:06Z
completed_at: 2026-07-27T05:26:10Z
actual_ms: 60000
---
# S-047: Shared table sort plumbing

## User story

As a user, I want consistent sort controls and behavior across board tables, so every list sorts the same way.

## Acceptance criteria

- [x] Shared sort key types cover at least `id`, `title`, `size`, and `epic`.
- [x] Pure comparators sort ascending/descending with stable, predictable handling of missing values.
- [x] A reusable sortable column header cycles none → asc → desc → none and shows the active direction.

## Tasks

- [T-142: Define sort keys, comparators, and types](items/T-142-sort-keys-comparators-types.md)
- [T-143: Build shared sortable table header UI](items/T-143-sortable-table-header-ui.md)
- [T-165: Three-click sort cycle clears to default](items/T-165-three-click-sort-clear.md)
- [T-166: Sort by points, status, and priority](items/T-166-sort-points-status-priority.md)
- [T-167: Sort by type and people](items/T-167-sort-type-and-people.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:19:23Z | prompt | Marco Mendão | Create stories and tasks for E-013 table sort (epic, size, title, id) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 4b6097c | taskmark-frontend | 2026-07-27T06:34:38+01:00 | Marco Mendão | add sortable table columns across board lists |
| f14af32 | taskmark-taskmark | 2026-07-27T06:34:38+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T05:20:06Z | 2026-07-27T05:20:06Z | — | Rollup: children hold shared-batch for E-013 |
