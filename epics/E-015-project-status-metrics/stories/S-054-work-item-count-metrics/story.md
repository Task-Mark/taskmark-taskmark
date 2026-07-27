---
id: S-054
type: story
title: Total and complete work item counts
status: done
priority: high
size: S
size_source: rolled_up
size_basis: [sum:tasks]
points: 3
points_source: rolled_up
estimate_minutes: 45
actual_minutes: 0
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-015
epic: E-015
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
tags: [frontend, metrics, counts]
created: 2026-07-27
updated: 2026-07-27T07:06:27.645Z
started_at: 2026-07-27T06:25:20Z
completed_at: 2026-07-27T06:28:48Z
actual_ms: 0
---
# S-054: Total and complete work item counts

## User story

As a project lead, I want to see how many stories, bugs, and tasks exist and how many are done, so I can gauge backlog volume and completion at a glance.

## Acceptance criteria

- [x] **Total work items** counts stories + bugs + tasks for the current board (epics excluded).
- [x] **Complete work items** counts the same types with `status: done` (cancelled excluded from both totals unless product already treats cancelled as non-work — document choice in Notes).
- [x] Counts update when the board data reloads / project switches.
- [x] Values render in the Total and Complete metric cards from S-053.

## Tasks

- [T-171: Aggregate total and done work item counts](items/T-171-aggregate-work-item-counts.md)
- [T-172: Wire count metrics into Total and Complete cards](items/T-172-wire-count-metric-cards.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 2 | 2026-07-27T06:25:20Z | prompt | Marco Mendão | Implement the E-015 |
| 1 | 2026-07-27T05:55:45Z | prompt | Marco Mendão | Create epic for project status metrics (total/complete/speed + contributors) styled like neo-brutalism metric cards; include stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:25:20Z | 2026-07-27T06:25:20Z | Parent rollup: children hold shared-batch |
