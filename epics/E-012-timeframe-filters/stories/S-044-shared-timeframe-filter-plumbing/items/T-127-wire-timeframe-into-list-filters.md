---
id: T-127
type: task
title: Wire timeframe into list filters and pagination
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
updated: 2026-07-27T05:16:43.229Z
started_at: 2026-07-24T16:02:37Z
completed_at: 2026-07-24T16:06:21Z
actual_ms: 32000
---
# T-127: Wire timeframe into list filters and pagination

## Description

Extend list filter composition so timeframe applies on epic, story, task, and work-items lists and resets page when changed.

## Acceptance criteria

- [x] Overall and Work items lists honor the active timeframe.
- [x] Changing timeframe resets to page 1.
- [x] Clearing timeframe restores unfiltered solved/open mix per other filters.

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
