---
id: S-047
type: story
title: Shared table sort plumbing
status: backlog
priority: medium
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 70
actual_minutes: 0
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
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, lists, sort]
created: 2026-07-24
updated: 2026-07-25T10:44:19.816Z
started_at: null
completed_at: null
actual_ms: 0
---

# S-047: Shared table sort plumbing

## User story

As a user, I want consistent sort controls and behavior across board tables, so every list sorts the same way.

## Acceptance criteria

- [ ] Shared sort key types cover at least `id`, `title`, `size`, and `epic`.
- [ ] Pure comparators sort ascending/descending with stable, predictable handling of missing values.
- [ ] A reusable sortable column header toggles asc ↔ desc and shows the active direction.

## Tasks

- [T-142: Define sort keys, comparators, and types](items/T-142-sort-keys-comparators-types.md)
- [T-143: Build shared sortable table header UI](items/T-143-sortable-table-header-ui.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:19:23Z | prompt | Marco Mendão | Create stories and tasks for E-013 table sort (epic, size, title, id) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
