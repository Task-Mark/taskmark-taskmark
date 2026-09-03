---
id: T-063
type: task
title: Build view switcher button group UI
status: done
priority: high
size: S
size_source: suggested
size_basis: [similar:list-ui]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-024
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
tags: [ui, frontend, views]
created: 2026-07-22
updated: 2026-09-03T21:43:00Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:39:10Z
actual_ms: 13000
---
# T-063: Build view switcher button group UI

## Description

Add a button-group (or equivalent segmented control) that lets the user switch between Overall, All, Stories, and Tasks views.

## Acceptance criteria

- [x] Switcher shows four labeled options: Overall, All, Stories, Tasks.
- [x] Selecting an option updates the active view mode.
- [x] Active option is visually indicated.
- [x] Control matches existing board UI primitives/styles.

## Notes

Prefer existing shadcn/ui ToggleGroup or Button group patterns if present.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T06:42:22Z | prompt | Marco Mendão | Implement E-006 |
| 3 | 2026-09-03T21:43:00Z | prompt | Marco Mendão | On mobile, local and Cloud boards should switch list views with a dropdown instead of tabs. |
| 2 | 2026-07-23T06:42:22Z | feedback | Marco Mendão | Shipped list view as part of E-006 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 2 | Marco Mendão | 2026-09-03T21:43:00Z | 2026-09-03T21:43:00Z | Replaced the list-view tabs with a dropdown below the mobile breakpoint. |
| 1 | Marco Mendão | 2026-07-23T06:38:57Z | 2026-07-23T06:39:10Z | shared-batch: 13667 of 205000ms by points |
