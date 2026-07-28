---
id: T-056
type: task
title: Wire epic list open to epic detail sheet
status: done
priority: high
size: S
size_source: suggested
size_basis: [calibrated:T-056]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: manual
estimate_basis: [manual:preserve-plan;burst-delivery]
session_cap_minutes: 480
parent: S-020
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
tags: [ui, epic, frontend, sheet]
created: 2026-07-21
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 12188
---

# T-056: Wire epic list open to epic detail sheet

## Description

Connect epic list open-detail actions to load epic full detail and render the epic layout inside the shared sheet.

## Acceptance criteria

- [x] Opening an epic from the list loads that epic’s detail and shows it in the sheet.
- [x] Loading/error states from S-018 appear for epic loads.
- [x] Existing epic selection for story drill-down still works.

## Notes

Depends on T-048–T-052 and T-055.

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
| 1 | Marco Mendão | 2026-07-21T23:53:57Z | 2026-07-21T23:54:09.188Z | Delivered as part of E-005; shared-batch: 12188 of 195000ms by points |
