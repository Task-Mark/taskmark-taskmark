---
id: T-049
type: task
title: Open sheet from epic story and task list rows
status: done
priority: high
size: S
size_source: suggested
size_basis: [calibrated:T-049]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: manual
estimate_basis: [manual:preserve-plan;burst-delivery]
session_cap_minutes: 480
parent: S-018
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
tags: [ui, sheet, frontend]
created: 2026-07-21
updated: 2026-07-27T05:37:38.663Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 12188
---

# T-049: Open sheet from epic story and task list rows

## Description

Add a clear open-detail affordance on epic, story, and task list rows that opens the shared sheet for that item, without replacing list selection / drill-down behavior.

## Acceptance criteria

- [x] Epic, story, and task lists can open the shared sheet for a chosen row.
- [x] Opening the sheet does not clear or break epic→story→task selection.
- [x] Only one work item sheet is open at a time; opening another replaces the viewed item.
- [x] Close returns to the same board context.

## Notes

Prefer an explicit view action (icon/button) if row click already selects for drill-down.

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
