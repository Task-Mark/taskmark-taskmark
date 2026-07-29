---
id: T-143
type: task
title: Build shared sortable table header UI
status: done
priority: medium
size: M
size_source: suggested
size_basis: [T-096, T-127]
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
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
updated: 2026-07-29T07:31:14.976Z
started_at: 2026-07-27T05:20:06Z
completed_at: 2026-07-27T05:22:17Z
actual_ms: 60000
---
# T-143: Build shared sortable table header UI

## Description

Reusable table header control that toggles sort direction and shows which column is active.

## Acceptance criteria

- [x] Clicking a sortable header cycles asc → desc → clear and updates the active key.
- [x] Active column shows a clear direction indicator; inactive sortable columns look clickable.
- [x] Control works with existing `TableHead` styling and basic keyboard focus/activation.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:19:23Z | prompt | Marco Mendão | Create stories and tasks for E-013 table sort (epic, size, title, id) |
| 99 | 2026-07-27T05:22:17Z | prompt | Marco Mendão | Implement this E-013 |
| 100 | 2026-07-27T05:22:17Z | feedback | Marco Mendão | Delivered as part of E-013 shared batch |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 4b6097c | taskmark-frontend | 2026-07-27T06:34:38+01:00 | Marco Mendão | add sortable table columns across board lists |
| f14af32 | taskmark-taskmark | 2026-07-27T06:34:38+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T05:20:06Z | 2026-07-27T05:21:06Z | — | SortableTableHead UI; shared-batch: 1 of 2min by points |
