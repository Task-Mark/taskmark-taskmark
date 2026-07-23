---
id: S-031
type: story
title: Collect and sort work items
status: backlog
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
parent: E-009
epic: E-009
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, views, workitems]
created: 2026-07-23
updated: 2026-07-23T06:35:04.706Z
started_at: null
completed_at: null
actual_ms: 0
---

# S-031: Collect and sort work items

## User story

As a user, I want the Work items list to include every story, task, and bug and to be ordered by status then priority so I can focus on what matters first.

## Acceptance criteria

- [ ] List includes all user stories, tasks, and bugs on the active project board (epics excluded).
- [ ] Primary order by status: `backlog`, then `in_progress` (progress), then `done`.
- [ ] Within the same status, order by priority (highest first; e.g. critical → high → medium → low).
- [ ] Cancelled / blocked items follow existing board conventions (include unless cancelled latch hides them).

## Tasks

- [T-085: Aggregate stories, tasks, and bugs into work item rows](items/T-085-aggregate-work-item-rows.md)
- [T-086: Sort work items by status then priority](items/T-086-sort-status-then-priority.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|

