---
id: T-107
type: task
title: Fix multiselect filter autocomplete
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-105]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 2
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-036
epic: E-010
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
tags: [dashboard, frontend, filters, bugfix]
created: 2026-07-23
updated: 2026-07-28T06:20:01.202Z
started_at: 2026-07-23T16:16:14Z
completed_at: 2026-07-23T16:18:24Z
actual_ms: 130000
---

# T-107: Fix multiselect filter autocomplete

## Description

Parent and tags multiselect comboboxes were not filtering the dropdown as the user typed. Wire Base UI `items` + list render-function so built-in list filtering works.

## Acceptance criteria

- [x] Typing in the parent picker filters the dropdown by id/title.
- [x] Typing in the tags picker filters the dropdown by tag text.
- [x] Empty query still shows the full option list; no-match shows empty state.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T16:16:14Z | prompt | Marco Mendão | multiselect filters autocomplete not working |
| 2 | 2026-07-23T16:18:24Z | feedback | Marco Mendão | items + list render filter wired |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 66b89f7 | taskmark-frontend | 2026-07-23T16:17:20Z | Marco Mendão | add list search and filters |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:16:14Z | 2026-07-23T16:18:24Z | Fixed Combobox items/list filtering for parent and tags |
