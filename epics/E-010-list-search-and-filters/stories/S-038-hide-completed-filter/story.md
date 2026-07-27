---
id: S-038
type: story
title: Hide completed filter
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 9
points_source: rolled_up
estimate_minutes: 135
actual_minutes: 3
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-010
epic: E-010
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
tags: [dashboard, frontend, filters]
created: 2026-07-23
updated: 2026-07-27T05:37:38.663Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-27T05:18:44Z
actual_ms: 205000
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
- [T-162: Persist each Hide completed toggle in a cookie](items/T-162-persist-hide-completed-cookies.md)
- [T-104: Compose filters with pagination reset](items/T-104-compose-filters-pagination.md)
- [B-006: Hide completed hides done epics that still have open epic-direct work](items/B-006-hide-completed-done-epic-open-direct.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T15:53:02Z | prompt | Marco Mendão | Epic for list search + parent/tag filters + hide completed; create stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:00:49Z | rollup: children hold shared-batch; delivered S-038 |
