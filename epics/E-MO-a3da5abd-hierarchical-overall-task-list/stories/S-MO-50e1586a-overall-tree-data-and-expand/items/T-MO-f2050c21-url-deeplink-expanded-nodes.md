---
id: T-MO-f2050c21
type: task
title: Deep-link Overall expand via epic and story query params
status: done
priority: high
size: S
points: 3
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
started_at: 2026-08-28T23:12:19Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-f2050c21: Deep-link Overall expand via epic and story query params

## Description

Keep `epic` and `story` search params as expand hints so shared URLs open the same nodes. Update links that previously meant “selected table row”.

## Acceptance criteria

- [x] Opening Overall with `epic` expands that epic.
- [x] Opening with `epic` and `story` expands both.
- [x] Invalid ids do not crash the list.


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
| Marco Mendão | 2026-08-28T23:12:19Z | 2026-08-28T23:12:48Z | epic/story URL params expand matching tree nodes. |

