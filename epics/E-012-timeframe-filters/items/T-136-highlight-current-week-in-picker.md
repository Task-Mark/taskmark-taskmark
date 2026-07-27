---
id: T-136
type: task
title: Highlight and quick-select current week in picker
status: done
priority: medium
size: XS
size_source: suggested
size_basis: [velocity:similar]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: E-012
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
tags: [filters, timeframe, weeks, frontend, ui]
created: 2026-07-24
updated: 2026-07-27T07:23:21.914Z
started_at: 2026-07-24T16:21:43Z
completed_at: 2026-07-24T16:22:23Z
actual_ms: 40000
---
# T-136: Highlight and quick-select current week in picker

## Description

In the week picker dropdown, visually distinguish the current ISO week and add a “This week” action that selects it.

## Acceptance criteria

- [x] Current week is visually distinct in the week list (badge / emphasis).
- [x] A “This week” button selects the current ISO week and closes the picker.

## Notes

Follow-up polish on E-012 / T-135.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T16:21:43Z | prompt | Marco Mendão | Distinguish current week in picker; add button to select current week |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T16:21:43Z | 2026-07-24T16:22:23Z | current week Now badge + This week quick select |
