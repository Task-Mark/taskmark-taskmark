---
id: T-143
type: task
title: Build shared sortable table header UI
status: backlog
priority: medium
size: M
size_source: suggested
size_basis: [T-096, T-127]
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 0
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
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, lists, sort]
created: 2026-07-24
updated: 2026-07-27T05:16:43.229Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-143: Build shared sortable table header UI

## Description

Reusable table header control that toggles sort direction and shows which column is active.

## Acceptance criteria

- [ ] Clicking a sortable header toggles asc ↔ desc and updates the active key.
- [ ] Active column shows a clear direction indicator; inactive sortable columns look clickable.
- [ ] Control works with existing `TableHead` styling and basic keyboard focus/activation.

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
