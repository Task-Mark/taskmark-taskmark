---
id: T-101
type: task
title: Parent epic/story autocomplete filter on Work items
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-071, T-096]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-036
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
updated: 2026-07-27T07:23:21.914Z
started_at: 2026-07-23T16:00:49Z
completed_at: 2026-07-23T16:03:09Z
actual_ms: 19000
---

# T-101: Parent epic/story autocomplete filter on Work items

## Description

Add an autocomplete dropdown on the Work items tab to filter rows by parent epic and/or story (type-ahead on id/title).

## Acceptance criteria

- [x] Options include epics and stories from the active board (labeled clearly).
- [x] Selecting an epic filters to rows under that epic; selecting a story filters to that story’s related rows (stories row itself and/or children as applicable to Work items row set).
- [x] Clearable; composes with search.

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
| 1 | Marco Mendão | 2026-07-23T16:00:49Z | 2026-07-23T16:01:08Z | shared-batch: 19189 of 140714ms by points; delivered T-101 |
