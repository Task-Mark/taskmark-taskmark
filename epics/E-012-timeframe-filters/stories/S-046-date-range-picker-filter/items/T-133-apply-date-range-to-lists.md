---
id: T-133
type: task
title: Apply date range filter to solved items on lists
status: done
priority: high
size: M
size_source: suggested
size_basis: [velocity:similar]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-046
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
tags: [filters, timeframe, date-range, frontend]
created: 2026-07-23
updated: 2026-07-27T05:37:38.663Z
started_at: 2026-07-24T16:02:37Z
completed_at: 2026-07-24T16:06:21Z
actual_ms: 32000
---

# T-133: Apply date range filter to solved items on lists

## Description

Filter Overall and Work items lists to items whose completed_at is within the inclusive date range.

## Acceptance criteria

- [x] Only items solved in the range are shown when the filter is active.
- [x] Open items without completed_at are excluded while the range is active.
- [x] Empty state when no matches.

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
| 1 | Marco Mendão | 2026-07-24T16:02:37Z | 2026-07-24T16:03:09Z | delivered; shared-batch: 32000 of 224000ms by points |
