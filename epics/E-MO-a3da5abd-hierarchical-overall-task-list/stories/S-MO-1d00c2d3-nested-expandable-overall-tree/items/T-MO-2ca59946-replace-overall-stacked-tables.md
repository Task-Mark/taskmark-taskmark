---
id: T-MO-2ca59946
type: task
title: Replace Overall stacked tables with one hierarchy
status: done
priority: high
size: L
points: 8
parent: S-MO-1d00c2d3
epic: E-MO-a3da5abd
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
blocked: false
cancelled: false
tags: [dashboard, frontend, overall]
created: 2026-08-29
updated: 2026-08-28T23:17:07Z
started_at: 2026-08-28T23:09:25Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-2ca59946: Replace Overall stacked tables with one hierarchy

## Description

Replace Overall on the live board and static board with a single nested list component. Remove the stacked EpicList + OverallWorkItemsList + TaskList layout for `view=overall`.

## Acceptance criteria

- [x] Overall no longer renders three independent tables for epics, work items, and sub-tasks.
- [x] All / Stories / Tasks still use their existing list components.
- [x] Heading copy no longer tells the user to select an epic to view work items.


## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-28T23:07:00Z | prompt | Marco Mendão | /tkmd-do E-MO-a3da5abd: replace Overall stacked tables with one hierarchical tree (live+static); tests; no commit/push. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-28T23:09:25Z | 2026-08-28T23:09:54Z | Replaced Overall stacked tables with OverallTreeList. |

