---
id: S-020
type: story
title: Epic detail view
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 80
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-005
epic: E-005
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
tags: [dashboard, frontend, epic, detail]
created: 2026-07-21
updated: 2026-07-24T16:49:37.998Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 30469
---

# S-020: Epic detail view

## User story

As a user, I want to open an epic in the sheet and see its details presented clearly so I understand goal, scope, and progress.

## Acceptance criteria

- [x] Epic sheet shows identity/meta (id, title, status, priority, points, est/actual, tags, dates) and body sections (goal, scope, out of scope, success metrics, stories, commits, work log).
- [x] Layout prioritizes readability for epic-shaped content (no cramped dump of raw markdown).
- [x] Opening an epic from the epic list loads and shows that epic’s detail in the sheet.

## Tasks

- [T-055: Build epic detail content layout](items/T-055-epic-detail-content-layout.md)
- [T-056: Wire epic list open to epic detail sheet](items/T-056-wire-epic-list-to-detail-sheet.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T23:48:59Z | prompt | Marco Mendão | Create all user stories and tasks for E-005 view work item |
| 2 | 2026-07-21T23:53:57Z | prompt | Marco Mendão | Develop epic E-005 — implement work item detail views in sheets |
| 3 | 2026-07-21T23:56:38Z | feedback | Marco Mendão | Implement E-005 detail sheets delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T23:53:57Z | 2026-07-21T23:53:57Z | Delivered as part of E-005; shared-batch: 0ms rollup (children hold allocation) |
