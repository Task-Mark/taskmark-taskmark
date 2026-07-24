---
id: T-088
type: task
title: Define pagination types and page-size defaults
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-062, T-085]
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
updated: 2026-07-24T17:39:50.198Z
started_at: 2026-07-23T15:35:42Z
completed_at: 2026-07-23T15:41:41Z
actual_ms: 47000
---
# T-088: Define pagination types and page-size defaults

## Description

Add shared TypeScript types and constants for list pagination: page (1-based), pageSize, allowed page sizes (e.g. 10, 25, 50, 100), and a default page size.

## Acceptance criteria

- [x] Exported types cover page, pageSize, and pagination state props.
- [x] Allowed page sizes and default are documented constants.
- [x] Defaults are usable by all list views without per-list magic numbers.

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
| 1 | Marco Mendão | 2026-07-23T15:35:42Z | 2026-07-23T15:36:29Z | shared-batch: 47891 of 359182ms by points; delivered T-088 |
