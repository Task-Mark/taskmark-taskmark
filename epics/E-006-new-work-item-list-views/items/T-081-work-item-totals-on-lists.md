---
id: T-081
type: task
title: Count work items (stories, tasks, bugs) on epic and story lists
status: done
priority: high
size: M
size_source: suggested
size_basis: [calibrated:T-081]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 3
estimate_source: suggested
estimate_basis: [calibrated:T-081]
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
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-23T06:25:29Z
completed_at: 2026-07-23T06:28:29Z
actual_ms: 180000
---

# T-081: Count work items (stories, tasks, bugs) on epic and story lists

## Description

Change the list totals column so it counts **work items**: user stories + tasks + bugs under an epic, and tasks + bugs under a story (no nested stories). Rename the column from Tasks to Work items.

## Acceptance criteria

- [x] Epic list Work items = count of stories under the epic + all tasks/bugs (story children and epic-direct).
- [x] Story list Work items = count of tasks and bugs under that story.
- [x] Column label is Work items (not Tasks).
- [x] Zero children show `0`.

## Notes

Follow-up to T-080. Frontend: `count-leaves.ts`, epic/story lists.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T06:25:29Z | prompt | Marco Mendão | Workitems = tasks + bugs + user stories under epic/story |
| 2 | 2026-07-23T06:26:02Z | feedback | Marco Mendão | Renamed to Work items; epic includes stories |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 3a96f58 | taskmark-frontend | 2026-07-23T06:27:22Z | Marco Mendão | add work item totals on lists |
| dcebe32 | taskmark-taskmark | 2026-07-23T06:27:22Z | Marco Mendão | complete t-080 t-081 list totals |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T06:25:29Z | 2026-07-23T06:28:29Z | Work items column counts stories+tasks+bugs |
