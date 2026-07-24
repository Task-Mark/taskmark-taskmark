---
id: T-131
type: task
title: Year dropdown and apply week filter to lists
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
updated: 2026-07-24T17:39:50.198Z
started_at: 2026-07-24T16:02:37Z
completed_at: 2026-07-24T16:06:21Z
actual_ms: 32000
---

# T-131: Year dropdown and apply week filter to lists

## Description

Add year dropdown (hidden when only one year) and apply year+week filter so only items solved in those weeks appear.

## Acceptance criteria

- [x] Single-year boards hide the year control.
- [x] Multi-year boards require/default a year selection.
- [x] Only items with completed_at in the selected weeks remain visible.

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
