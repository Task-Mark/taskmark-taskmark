---
id: T-142
type: task
title: Define sort keys, comparators, and types
status: backlog
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
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, lists, sort]
created: 2026-07-24
updated: 2026-07-24T17:39:50.198Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-142: Define sort keys, comparators, and types

## Description

Add shared TypeScript types and pure comparators for table sort keys (`id`, `title`, `size`, `epic`) and direction (asc/desc).

## Acceptance criteria

- [ ] Exported `SortKey` / `SortDirection` (or equivalent) cover id, title, size, and epic.
- [ ] Comparators are pure, deterministic, and treat missing/null values consistently (e.g. last on asc).
- [ ] Size compare uses t-shirt order (XS < S < M < L < XL), not alphabetical.
- [ ] Id compare is natural for Taskmark ids (prefix then numeric) when that improves ordering.

## Notes

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
