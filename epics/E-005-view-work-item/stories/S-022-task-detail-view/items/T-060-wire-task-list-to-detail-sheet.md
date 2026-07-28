---
id: T-060
type: task
title: Wire task list open to item detail sheet
status: done
priority: high
size: S
size_source: suggested
size_basis: [calibrated:T-060]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: manual
estimate_basis: [manual:preserve-plan;burst-delivery]
session_cap_minutes: 480
parent: S-022
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
tags: [ui, tasks, frontend, sheet]
created: 2026-07-21
updated: 2026-07-28T09:08:49.505Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 12187
---

# T-060: Wire task list open to item detail sheet

## Description

Connect task list open-detail actions to load task/bug full detail and render the item layout inside the shared sheet.

## Acceptance criteria

- [x] Opening a task or bug from the list loads that item’s detail and shows it in the sheet.
- [x] Loading/error states from S-018 appear for item loads.
- [x] Existing task list selection behavior is preserved.

## Notes

Depends on T-048–T-051, T-054, and T-059.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T23:48:59Z | prompt | Marco Mendão | Create all user stories and tasks for E-005 view work item |
| 2 | 2026-07-21T23:56:38Z | feedback | Marco Mendão | Implement E-005 detail sheets delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T23:53:57Z | 2026-07-21T23:54:09.187Z | Delivered as part of E-005; shared-batch: 12187 of 195000ms by points |
