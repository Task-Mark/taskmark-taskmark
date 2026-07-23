---
id: T-080
type: task
title: Add task and bug totals on epic and story lists
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-006, T-012]
points: 3
points_source: suggested
estimate_minutes: 45
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: E-006
epic: E-006
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, lists]
created: 2026-07-23
updated: 2026-07-23T05:40:52Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-080: Add task and bug totals on epic and story lists

## Description

Show a combined **Tasks** total (tasks + bugs counted together in one column) on each row of the epics list and each row of the stories list, so users can see leaf volume without opening every child.

## Acceptance criteria

- [ ] Epic list has a column (or equivalent cell) showing the total count of tasks and bugs under that epic (story children + epic-direct leaves).
- [ ] Story list has the same style of column showing the total count of tasks and bugs under that story.
- [ ] Tasks and bugs share one total (not separate columns).
- [ ] Zero children show `0` (or an agreed empty display), not a blank/crash.
- [ ] Totals update correctly when switching project / selecting another epic.

## Notes

Overall drill-down lists: `epic-list.tsx` and `story-list.tsx`. Count leaf markdown under the epic (all descendant tasks/bugs) and under each story’s `items/`.

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-23T05:40:03Z | prompt | Add totals of tasks+bugs (same column) on epic list and stories list |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| d5eb379 | taskmark-taskmark | 2026-07-23T05:40:41Z | add t-080 list totals task |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
