---
id: S-032
type: story
title: Paginate Work items list
status: done
priority: high
size: S
size_source: rolled_up
size_basis: [sum:tasks]
points: 2
points_source: rolled_up
estimate_minutes: 30
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-009
epic: E-009
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
tags: [dashboard, frontend, pagination, workitems]
created: 2026-07-23
updated: 2026-07-24T16:57:53.518Z
started_at: 2026-07-23T15:35:42Z
completed_at: 2026-07-23T15:41:41Z
actual_ms: 47000
---

# S-032: Paginate Work items list

## User story

As a user on the Work items tab, I want the mixed stories / epic-direct tasks table paginated with the shared control, so large flat lists stay manageable.

## Acceptance criteria

- [x] Work items list shows only the current page of rows.
- [x] Shared pagination control (nav + page size) is visible when there is at least one row (or always, disabled when empty — either is OK if consistent).
- [x] Sort order (status → priority → created) is preserved before slicing.
- [x] Opening a detail sheet from a paginated row still works.

## Tasks

- [T-094: Paginate work items list](items/T-094-paginate-work-items-list.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T15:29:50Z | prompt | Marco Mendão | Create epic for list pagination with nav + page size; include stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T15:35:42Z | 2026-07-23T15:35:42Z | shared-batch parent rollup (0 min); leaves hold effort |
