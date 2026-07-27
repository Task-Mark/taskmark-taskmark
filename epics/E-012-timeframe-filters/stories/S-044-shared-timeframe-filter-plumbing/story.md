---
id: S-044
type: story
title: Shared timeframe filter plumbing
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 7
points_source: rolled_up
estimate_minutes: 110
actual_minutes: 1
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-012
epic: E-012
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
tags: [filters, timeframe, frontend]
created: 2026-07-23
updated: 2026-07-27T05:37:38.663Z
started_at: 2026-07-24T16:02:37Z
completed_at: 2026-07-24T16:06:21Z
actual_ms: 74667
---

# S-044: Shared timeframe filter plumbing

## User story

As a board viewer, I want shared timeframe filter state and solved-date matching so year/week and date-range controls can filter every list consistently.

## Acceptance criteria

- [x] Shared types/state for active timeframe mode (none | weeks | range).
- [x] Helpers match an item’s completed_at (solved date) against ISO week ranges and calendar date ranges.
- [x] Filters compose with search, hide-completed, parent/tags, and reset pagination to page 1 when the timeframe changes.
- [x] Wired into Overall and Work items list surfaces.

## Tasks

- [T-126: Define timeframe filter types and solved-date helpers](items/T-126-timeframe-filter-types-and-helpers.md)
- [T-127: Wire timeframe into list filters and pagination](items/T-127-wire-timeframe-into-list-filters.md)
- [T-128: Add timeframe controls slot to list filters bar](items/T-128-timeframe-filter-bar-slot.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T16:02:37Z | 2026-07-24T16:02:37Z | rollup: children hold shared-batch; delivered story |
