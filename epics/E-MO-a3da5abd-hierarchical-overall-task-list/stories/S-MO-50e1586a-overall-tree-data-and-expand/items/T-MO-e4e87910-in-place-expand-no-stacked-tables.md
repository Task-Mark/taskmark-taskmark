---
id: T-MO-e4e87910
type: task
title: Expand children in place instead of extra tables
status: done
priority: high
size: M
points: 5
parent: S-MO-50e1586a
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
started_at: 2026-08-28T23:11:50Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-e4e87910: Expand children in place instead of extra tables

## Description

Wire the Overall UI so expand toggles child rows in the same component. Delete the select-epic-then-scroll-to-work-items-then-select-story flow.

## Acceptance criteria

- [x] Expanding does not mount OverallWorkItemsList or TaskList as sibling sections under Overall.
- [x] Collapse hides children without a full navigation reset.


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
| Marco Mendão | 2026-08-28T23:11:50Z | 2026-08-28T23:12:19Z | In-place expand/collapse; no sibling OverallWorkItemsList/TaskList. |

