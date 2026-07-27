---
id: T-129
type: task
title: Derive available years and week bounds from board
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
parent: S-045
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
tags: [filters, timeframe, weeks, frontend]
created: 2026-07-23
updated: 2026-07-27T07:09:18.868Z
started_at: 2026-07-24T16:02:37Z
completed_at: 2026-07-24T16:06:21Z
actual_ms: 21333
---

# T-129: Derive available years and week bounds from board

## Description

Scan parsed work items’ completed_at to build the set of years and min/max ISO week per year.

## Acceptance criteria

- [x] Years list is sorted ascending.
- [x] Week bounds for a year reflect data in that year (fallback 1–52/53 when empty).
- [x] Items without completed_at do not contribute years.

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
| 1 | Marco Mendão | 2026-07-24T16:02:37Z | 2026-07-24T16:02:58.333Z | delivered; shared-batch: 21333 of 224000ms by points |
