---
id: T-MM-ae1cf7c4
type: task
title: Global project, author, and timeframe filters
status: backlog
priority: high
size: M
points: 5
parent: S-MM-46b6e806
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, frontend, filters]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-ae1cf7c4: Global project, author, and timeframe filters

## Description

Client wrapper in `taskmark-cloud/components/dashboard/` that owns the shared filter state and passes filtered data to every widget. Project and author multi-selects follow the `tags-multiselect-filter` pattern from `@taskmark/components`; authors are derived from worklog actors and contributors across all projects. Timeframe reuses `TimeframeFilter` and the ISO-week/date-range helpers in `timeframe-filters.ts`.

## Acceptance criteria

- [ ] Projects and authors can each be narrowed with a multi-select showing all available values from the payload.
- [ ] Timeframe supports ISO weeks and date ranges exactly like the board views.
- [ ] Changing any filter updates every widget on the page without a server round trip.
- [ ] Clearing filters restores the full aggregated view.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — global filters by project, author, and timeframe. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
