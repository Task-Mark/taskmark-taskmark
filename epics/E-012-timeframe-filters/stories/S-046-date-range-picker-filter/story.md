---
id: S-046
type: story
title: Date range picker filter
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 6
points_source: rolled_up
estimate_minutes: 100
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
tags: [filters, timeframe, date-range, frontend]
created: 2026-07-23
updated: 2026-07-27T06:17:22.249Z
started_at: 2026-07-24T16:02:37Z
completed_at: 2026-07-24T16:06:21Z
actual_ms: 64000
---

# S-046: Date range picker filter

## User story

As a board viewer, I want to pick a from/to date range so I only see work items solved between those dates.

## Acceptance criteria

- [x] Date range picker lets the user choose two dates (from and to).
- [x] Lists show only epics/stories/tasks/bugs whose completed_at falls within the inclusive range.
- [x] Clearing the range removes the date-range timeframe filter.
- [x] Works alongside or as an alternative mode to the year/week filter (clear mutual exclusivity or documented composition).

## Tasks

- [T-132: Build date range picker UI](items/T-132-date-range-picker-ui.md)
- [T-133: Apply date range filter to solved items on lists](items/T-133-apply-date-range-to-lists.md)

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
