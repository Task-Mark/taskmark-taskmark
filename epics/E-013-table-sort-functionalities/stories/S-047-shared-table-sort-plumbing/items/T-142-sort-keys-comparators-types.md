---
id: T-142
type: task
title: Define sort keys, comparators, and types
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-095, T-126]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-047
epic: E-013
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
tags: [dashboard, frontend, lists, sort]
created: 2026-07-24
updated: 2026-08-14T17:50:46.835Z
started_at: 2026-07-27T05:20:06Z
completed_at: 2026-07-27T05:22:17Z
actual_ms: 0
---

# T-142: Define sort keys, comparators, and types

## Description

Add shared TypeScript types and pure comparators for table sort keys (`id`, `title`, `size`, `epic`) and direction (asc/desc).

## Acceptance criteria

- [x] Exported `SortKey` / `SortDirection` (or equivalent) cover id, title, size, and epic.
- [x] Comparators are pure, deterministic, and treat missing/null values consistently (e.g. last on asc).
- [x] Size compare uses t-shirt order (XS < S < M < L < XL), not alphabetical.
- [x] Id compare is natural for Taskmark ids (prefix then numeric) when that improves ordering.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:19:23Z | prompt | Marco Mendão | Create stories and tasks for E-013 table sort (epic, size, title, id) |
| 2 | 2026-07-27T05:20:06Z | prompt | Marco Mendão | Implement this E-013 |
| 3 | 2026-07-27T05:22:17Z | feedback | Marco Mendão | Delivered as part of E-013 shared batch |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 4b6097c | taskmark-frontend | 2026-07-27T06:34:38+01:00 | Marco Mendão | add sortable table columns across board lists |
| f14af32 | taskmark-taskmark | 2026-07-27T06:34:38+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T05:20:06Z | 2026-07-27T05:20:06Z | — | Sort keys, comparators, types; shared-batch: 0 of 2min by points |
