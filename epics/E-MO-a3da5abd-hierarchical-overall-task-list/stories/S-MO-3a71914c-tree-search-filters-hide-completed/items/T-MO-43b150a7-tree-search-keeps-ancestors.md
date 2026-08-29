---
id: T-MO-43b150a7
type: task
title: Search the tree and keep ancestor context
status: done
priority: high
size: M
points: 5
parent: S-MO-3a71914c
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
started_at: 2026-08-28T23:13:46Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-43b150a7: Search the tree and keep ancestor context

## Description

Overall search filters the tree: matching nodes stay visible with their ancestors. Non-matching branches collapse out of the result set.

## Acceptance criteria

- [x] A task title match shows its story and epic.
- [x] Unrelated epics disappear from the filtered tree.


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
| Marco Mendão | 2026-08-28T23:13:46Z | 2026-08-28T23:14:15Z | Search keeps matching descendants' ancestors. |

