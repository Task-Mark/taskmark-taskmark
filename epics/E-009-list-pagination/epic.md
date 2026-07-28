---
id: E-009
type: epic
title: List pagination for work items
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 15
points_source: rolled_up
estimate_minutes: 230
actual_minutes: 13
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
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
tags: [dashboard, frontend, lists, pagination]
created: 2026-07-23
updated: 2026-07-28T07:41:00.094Z
started_at: 2026-07-23T15:35:42Z
completed_at: 2026-07-23T15:41:41Z
actual_ms: 808000
---
# E-009: List pagination for work items

## Goal

Every work-item list in the system (Overall epic/story/task tables and the Work items list) supports pagination with first / previous / next / last navigation and a page-size dropdown so large boards stay usable.

## Scope

- Shared pagination control: first, previous, next, last; current page indicator; page-size select.
- Apply pagination to Overall epic, story, and task lists.
- Apply pagination to the Work items tab list.
- Sensible default page sizes and disabled nav when at bounds.

## Out of scope

- Server-side / filesystem streaming pagination (client-side slice of already-loaded rows is enough).
- Infinite scroll.
- Persisting page index across navigation (page size persistence optional later).
- Paginating detail-sheet children lists.

## Success metrics

- User can change page size and move between pages on every main list.
- Nav controls disable correctly on first/last page.
- Empty and short lists still render cleanly (no broken controls).

## Stories

- [S-030: Shared pagination control](stories/S-030-shared-pagination-control/story.md)
- [S-031: Paginate Overall drill-down lists](stories/S-031-paginate-overall-lists/story.md)
- [S-032: Paginate Work items list](stories/S-032-paginate-work-items-list/story.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 7bd7ab2 | taskmark-frontend | 2026-07-23T15:49:09Z | Marco Mendão | add list pagination controls |
| 1245518 | taskmark-taskmark | 2026-07-23T15:49:10Z | Marco Mendão | complete e-009 list pagination board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T15:35:42Z | 2026-07-23T15:35:42Z | shared-batch parent rollup (0 min); leaves hold effort |
| 2 | Marco Mendão | 2026-07-23T15:35:42Z | 2026-07-23T15:49:10Z | auto-recovered: commit span |
