---
id: T-095
type: task
title: Define search match helpers and filter types
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-088, T-090]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-033
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
tags: [dashboard, frontend, search]
created: 2026-07-23
updated: 2026-07-24T17:14:20.339Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-23T16:03:09Z
actual_ms: 12000
---
# T-095: Define search match helpers and filter types

## Description

Add shared TypeScript helpers/types for list search: normalize query, match against `id` and `title`, and shared filter-state shapes used by later stories.

## Acceptance criteria

- [x] `matchesWorkItemSearch(query, { id, title })` returns true for empty query or case-insensitive substring on id or title.
- [x] Exported types cover search query string and optional filter flags for reuse.
- [x] Helpers are pure and unit-testable without React.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T16:03:09Z | prompt | Marco Mendão | implement E-010 list search and filters |
| 2 | 2026-07-23T16:03:09Z | feedback | Marco Mendão | delivered search, parent/tags filters, hide completed |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:01:01Z | shared-batch: 12792 of 140714ms by points; delivered T-095 |
