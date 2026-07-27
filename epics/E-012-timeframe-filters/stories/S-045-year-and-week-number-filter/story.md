---
id: S-045
type: story
title: Year and week number filter
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 8
points_source: rolled_up
estimate_minutes: 130
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
tags: [filters, timeframe, weeks, frontend]
created: 2026-07-23
updated: 2026-07-27T07:45:28.202Z
started_at: 2026-07-24T16:02:37Z
completed_at: 2026-07-24T16:06:21Z
actual_ms: 85333
---

# S-045: Year and week number filter

## User story

As a board viewer, I want to pick a year and week-number range so I only see work items solved in those weeks.

## Acceptance criteria

- [x] Year dropdown lists years derived from board completed_at values.
- [x] If the board has only one year, the year dropdown is hidden and only the week slider is shown.
- [x] Week numbers are selected via a range slider for the active year.
- [x] Lists show only epics/stories/tasks/bugs whose completed_at falls in the selected weeks.

## Tasks

- [T-129: Derive available years and week bounds from board](items/T-129-derive-years-and-week-bounds.md)
- [T-130: Build week number range slider UI](items/T-130-week-number-range-slider.md)
- [T-131: Year dropdown and apply week filter to lists](items/T-131-year-dropdown-and-week-filter.md)

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
