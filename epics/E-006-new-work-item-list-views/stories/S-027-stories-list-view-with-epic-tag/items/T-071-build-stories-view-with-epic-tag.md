---
id: T-071
type: task
title: Build Stories view table with epic tag
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
parent: S-027
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
tags: [ui, frontend, views, stories]
created: 2026-07-22
updated: 2026-07-27T07:45:28.202Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:39:10Z
actual_ms: 13000
---
# T-071: Build Stories view table with epic tag

## Description

Render a stories-only table/list where each row shows an epic tag (badge/chip) identifying the parent epic.

## Acceptance criteria

- [x] Stories view shows only stories (no epics or tasks).
- [x] Each row displays an epic tag for the parent epic.
- [x] Core story fields (id, title, status, timing) remain visible.

## Notes

Tag means a UI badge for the parent epic, not Taskmark frontmatter tags.

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
