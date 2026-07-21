---
id: T-049
type: task
title: Open sheet from epic story and task list rows
status: backlog
priority: high
size: S
size_source: suggested
size_basis: [T-016, T-013]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-018
epic: E-005
owner: ""
blocked: false
cancelled: false
tags: [ui, sheet, frontend]
created: 2026-07-21
updated: 2026-07-21T23:50:12Z
started_at: null
completed_at: null
---

# T-049: Open sheet from epic story and task list rows

## Description

Add a clear open-detail affordance on epic, story, and task list rows that opens the shared sheet for that item, without replacing list selection / drill-down behavior.

## Acceptance criteria

- [ ] Epic, story, and task lists can open the shared sheet for a chosen row.
- [ ] Opening the sheet does not clear or break epic→story→task selection.
- [ ] Only one work item sheet is open at a time; opening another replaces the viewed item.
- [ ] Close returns to the same board context.

## Notes

Prefer an explicit view action (icon/button) if row click already selects for drill-down.

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T23:48:59Z | prompt | Create all user stories and tasks for E-005 view work item |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
