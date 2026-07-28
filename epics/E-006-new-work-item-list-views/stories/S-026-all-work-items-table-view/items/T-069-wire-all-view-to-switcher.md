---
id: T-069
type: task
title: Wire All view into switcher and detail sheet
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
parent: S-026
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
tags: [frontend, views, all, sheet]
created: 2026-07-22
updated: 2026-07-28T07:27:54.696Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:39:10Z
actual_ms: 13000
---

# T-069: Wire All view into switcher and detail sheet

## Description

Show the All table when All is selected; row activation opens the existing work item detail sheet for that item.

## Acceptance criteria

- [x] Selecting All in the switcher shows the unified table.
- [x] Clicking/activating a row opens the correct detail sheet for that item type.
- [x] Closing the sheet returns to the All table context.

## Notes



## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T06:42:22Z | prompt | Marco Mendão | Implement E-006 |
| 2 | 2026-07-23T06:42:22Z | feedback | Marco Mendão | Shipped list view as part of E-006 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T06:38:57Z | 2026-07-23T06:39:10Z | shared-batch: 13667 of 205000ms by points |
