---
id: T-082
type: task
title: Overall and Work items tabs only
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-068, T-071]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 3
estimate_source: suggested
estimate_basis: [calibrated:T-082]
session_cap_minutes: 480
parent: E-006
epic: E-006
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
tags: [dashboard, frontend, views, workitems]
created: 2026-07-23
updated: 2026-07-27T05:16:43.229Z
started_at: 2026-07-23T07:00:14Z
completed_at: 2026-07-23T07:03:14Z
actual_ms: 180000
---

# T-082: Overall and Work items tabs only

## Description

Replace the four list-view tabs with **Overall** and **Work items**. Work items shows stories plus epic-direct tasks/bugs (exclude tasks/bugs under a story), with priority column, sorted by status then priority. No Work items count column.

## Acceptance criteria

- [x] Board switcher has only Overall and Work items.
- [x] Work items lists stories, tasks, and bugs.
- [x] Tasks/bugs that belong to a story are not listed (epic-direct only).
- [x] No Work items count column on this tab.
- [x] Priority column is shown.
- [x] Rows ordered by status (backlog → in_progress → done) then by priority (highest first), then by created date (newest first).

## Notes

Supersedes All / Stories / Tasks as separate tabs from E-006; keeps Overall drill-down.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T07:00:14Z | prompt | Marco Mendão | Two tabs Overall + Work items; mix stories/tasks; no story children; priority sort |

| 2 | 2026-07-23T07:04:52Z | prompt | Marco Mendão | Tertiary sort by creating date |

| 3 | 2026-07-23T07:05:44Z | prompt | Marco Mendão | Created sort newest first |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 97685ee | taskmark-frontend | 2026-07-23T07:08:21Z | Marco Mendão | add overall and work items views |
| ce68818 | taskmark-taskmark | 2026-07-23T07:08:22Z | Marco Mendão | complete e-006 work items tabs |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T07:00:14Z | 2026-07-23T07:03:14Z | Overall + Work items tabs; epic-direct only; status/priority sort |
