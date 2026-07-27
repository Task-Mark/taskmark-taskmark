---
id: S-036
type: story
title: Parent epic/story autocomplete filter
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 6
points_source: rolled_up
estimate_minutes: 95
actual_minutes: 4
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
tags: [dashboard, frontend, filters, workitems]
created: 2026-07-23
updated: 2026-07-27T05:30:10.150Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-23T16:18:24Z
actual_ms: 279000
---
# S-036: Parent epic/story autocomplete filter

## User story

As a user on Work items, I want an autocomplete dropdown to filter by parent epic or story, so I can focus on one branch of the hierarchy.

## Acceptance criteria

- [x] Autocomplete lists epics and stories available on the board (id + title).
- [x] Selecting a parent filters Work items rows to that epic and/or story.
- [x] Clearing the selection removes the parent filter.
- [x] Works together with search and pagination.
- [x] Parent picker is multiselect (match any selected epic or story).

## Tasks

- [T-101: Parent epic/story autocomplete filter on Work items](items/T-101-parent-autocomplete-filter.md)
- [T-105: Parent filter multiselect and search chips layout](items/T-105-parent-multiselect-search-layout.md)
- [T-107: Fix multiselect filter autocomplete](items/T-107-fix-multiselect-autocomplete.md)

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
| 1 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:00:49Z | rollup: children hold shared-batch; delivered S-036 |
