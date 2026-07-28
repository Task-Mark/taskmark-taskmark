---
id: T-080
type: task
title: Add task and bug totals on epic and story lists
status: done
priority: high
size: S
size_source: suggested
size_basis: [calibrated:T-080]
points: 2
points_source: suggested
estimate_minutes: 50
actual_minutes: 49
estimate_source: suggested
estimate_basis: [calibrated:T-080]
session_cap_minutes: 480
parent: E-006
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
tags: [dashboard, frontend, lists]
created: 2026-07-23
updated: 2026-07-28T06:20:01.202Z
started_at: 2026-07-23T05:44:00Z
completed_at: 2026-07-23T05:47:00Z
actual_ms: 2981000
---
# T-080: Add task and bug totals on epic and story lists

## Description

Show a combined **Tasks** total (tasks + bugs counted together in one column) on each row of the epics list and each row of the stories list, so users can see leaf volume without opening every child.

## Acceptance criteria

- [x] Epic list has a column (or equivalent cell) showing the total count of tasks and bugs under that epic (story children + epic-direct leaves).
- [x] Story list has the same style of column showing the total count of tasks and bugs under that story.
- [x] Tasks and bugs share one total (not separate columns).
- [x] Zero children show `0` (or an agreed empty display), not a blank/crash.
- [x] Totals update correctly when switching project / selecting another epic.

## Notes

Overall drill-down lists: `epic-list.tsx` and `story-list.tsx`. Count leaf markdown under the epic (all descendant tasks/bugs) and under each story’s `items/`.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T05:40:03Z | prompt | Marco Mendão | Add totals of tasks+bugs (same column) on epic list and stories list |
| 2 | 2026-07-23T05:44:00Z | prompt | Marco Mendão | Implement T-080 |
| 3 | 2026-07-23T05:46:18Z | feedback | Marco Mendão | Shipped Tasks totals on epic-list and story-list |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| d5eb379 | taskmark-taskmark | 2026-07-23T05:40:41Z | Marco Mendão | add t-080 list totals task |
| 3a96f58 | taskmark-frontend | 2026-07-23T06:27:22Z | Marco Mendão | add work item totals on lists |
| dcebe32 | taskmark-taskmark | 2026-07-23T06:27:22Z | Marco Mendão | complete t-080 t-081 list totals |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T05:44:00Z | 2026-07-23T05:47:00Z | Added Tasks column (tasks+bugs) on epic and story lists |
| 2 | Marco Mendão | 2026-07-23T05:40:41Z | 2026-07-23T06:27:22Z | auto-recovered: commit span |
