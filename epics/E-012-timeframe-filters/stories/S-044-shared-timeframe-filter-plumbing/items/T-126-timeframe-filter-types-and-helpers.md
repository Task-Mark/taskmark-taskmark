---
id: T-126
type: task
title: Define timeframe filter types and solved-date helpers
status: done
priority: high
size: S
size_source: suggested
size_basis: [velocity:similar]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-044
epic: E-012
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
tags: [filters, timeframe, frontend]
created: 2026-07-23
updated: 2026-07-25T10:24:50.747Z
started_at: 2026-07-24T16:02:37Z
completed_at: 2026-07-24T16:06:21Z
actual_ms: 21334
---
# T-126: Define timeframe filter types and solved-date helpers

## Description

Add shared types for timeframe mode and helpers that parse completed_at and test membership in an ISO week span or inclusive date range.

## Acceptance criteria

- [x] Helpers accept completed_at ISO/date strings and return boolean match.
- [x] ISO week numbering is documented (ISO-8601).
- [x] Missing completed_at never matches an active timeframe filter.

## Notes

Solved date = frontmatter `completed_at`.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T16:06:21Z | prompt | Marco Mendão | implement E-012 timeframe filters |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T16:02:37Z | 2026-07-24T16:02:58.334Z | delivered; shared-batch: 21334 of 224000ms by points |
