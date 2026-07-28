---
id: T-090
type: task
title: Client-side page slice helper
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-067, T-088]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-030
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
tags: [dashboard, frontend, pagination]
created: 2026-07-23
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-23T15:35:42Z
completed_at: 2026-07-23T15:41:41Z
actual_ms: 47000
---
# T-090: Client-side page slice helper

## Description

Provide a pure helper that, given rows + page + pageSize, returns the current page slice plus totalPages / totalCount, clamping invalid page indexes.

## Acceptance criteria

- [x] Helper returns `{ pageRows, totalCount, totalPages, page }` with a valid clamped page.
- [x] Empty input yields totalPages 0 or 1 with empty pageRows (document chosen behavior).
- [x] Changing pageSize with an out-of-range page clamps safely.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T15:35:42Z | prompt | Marco Mendão | Implement epic E-009 list pagination |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T15:35:42Z | 2026-07-23T15:36:29Z | shared-batch: 47891 of 359182ms by points; delivered T-090 |
