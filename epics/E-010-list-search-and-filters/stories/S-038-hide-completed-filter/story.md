---
id: S-038
type: story
title: Hide completed filter
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 75
actual_minutes: 2
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-010
epic: E-010
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, filters]
created: 2026-07-23
updated: 2026-07-23T16:33:36.080Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-23T16:16:45Z
actual_ms: 154000
---
# S-038: Hide completed filter

## User story

As a user, I want to hide completed epics, stories, and tasks/bugs, so open work stays visible without noise from done items.

## Acceptance criteria

- [x] A control toggles hiding rows with status `done` (and optionally `cancelled` — document; prefer hide `done` only unless cancelled is clearly “complete”).
- [x] Applies to Overall epic, story, and task lists and to Work items.
- [x] Composes with search/parent/tag filters; resets pagination when toggled.
- [x] Shared filter state helpers avoid duplicating logic per list.

## Tasks

- [T-103: Hide completed control on all lists](items/T-103-hide-completed-filter.md)
- [T-106: Hide completed control as switch](items/T-106-hide-completed-switch.md)
- [T-104: Compose filters with pagination reset](items/T-104-compose-filters-pagination.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-23T15:53:02Z | prompt | Epic for list search + parent/tag filters + hide completed; create stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-23T16:00:49Z | 2026-07-23T16:00:49Z | rollup: children hold shared-batch; delivered S-038 |
