---
id: T-MO-d2152cb0
type: task
title: Paginate Overall by root epics
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
started_at: 2026-08-28T23:13:17Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-d2152cb0: Paginate Overall by root epics

## Description

If Overall stays paginated, page epic roots. Children of an epic on the page are not split across pages.

## Acceptance criteria

- [x] Page size applies to root epics, not flattened rows.
- [x] Expanding an epic does not jump the user to another page for its children.


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
| Marco Mendão | 2026-08-28T23:13:17Z | 2026-08-28T23:13:46Z | Pagination applies to root epics only. |

