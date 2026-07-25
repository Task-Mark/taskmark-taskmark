---
id: S-022
type: story
title: Task and bug detail view
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
tags: [dashboard, frontend, tasks, detail]
created: 2026-07-21
updated: 2026-07-25T10:24:50.747Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 30468
---

# S-022: Task and bug detail view

## User story

As a user, I want to open a task or bug in the sheet and see its details presented clearly so I can review description, criteria, and activity history.

## Acceptance criteria

- [x] Task/bug sheet shows identity/meta (including type) and body sections appropriate to type (description + AC for tasks; description + repro + fix criteria for bugs; notes; prompt & feedback; commits; work log).
- [x] Layout prioritizes readability and clearly distinguishes bugs from tasks.
- [x] Opening an item from the task list loads and shows that item’s detail in the sheet.

## Tasks

- [T-059: Build task and bug detail content layout](items/T-059-task-bug-detail-content-layout.md)
- [T-060: Wire task list open to item detail sheet](items/T-060-wire-task-list-to-detail-sheet.md)

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
