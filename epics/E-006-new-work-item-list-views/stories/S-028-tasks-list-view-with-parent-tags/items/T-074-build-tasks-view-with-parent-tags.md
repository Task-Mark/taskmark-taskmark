---
id: T-074
type: task
title: Build Tasks view table with epic and story tags
status: done
priority: high
size: M
size_source: suggested
size_basis: [similar:list-ui]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-028
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
tags: [ui, frontend, views, tasks]
created: 2026-07-22
updated: 2026-07-27T07:09:18.868Z
started_at: 2026-07-23T06:38:57Z
completed_at: 2026-07-23T06:39:17Z
actual_ms: 20000
---

# T-074: Build Tasks view table with epic and story tags

## Description

Render a tasks-only table where each row shows tags for the parent epic and parent story.

## Acceptance criteria

- [x] Tasks view shows only tasks/bugs (no epics or stories as primary rows).
- [x] Each row displays an epic tag and a story tag.
- [x] Type distinction between task and bug remains clear.
- [x] Core fields (id, title, status, timing) remain visible.

## Notes

Tags are UI badges for parent epic/story, not frontmatter tag lists.

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
| 1 | Marco Mendão | 2026-07-23T06:38:57Z | 2026-07-23T06:39:17Z | shared-batch: 20500 of 205000ms by points |
