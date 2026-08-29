---
id: T-MO-dd309a8b
type: task
title: Apply timeframe filter to the Overall tree
status: done
priority: high
size: S
points: 3
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
started_at: 2026-08-28T23:14:44Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-dd309a8b: Apply timeframe filter to the Overall tree

## Description

Reuse the existing timeframe control on Overall so the tree respects the same completion window rules as today’s lists.

## Acceptance criteria

- [x] Timeframe can hide nodes outside the window.
- [x] Ancestors of a matching descendant remain visible when needed for context.


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
| Marco Mendão | 2026-08-28T23:14:44Z | 2026-08-28T23:15:13Z | Timeframe filter keeps ancestor context for matching leaves. |

