---
id: T-MO-5a22506f
type: task
title: Shared incomplete-then-newest sort comparator
status: done
priority: high
size: S
points: 3
parent: S-MO-bb8f7f8b
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
started_at: 2026-08-28T23:07:00Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-5a22506f: Shared incomplete-then-newest sort comparator

## Description

Add a reusable comparator: incomplete statuses before complete/cancelled; then `created` descending; then `updated` descending; then id for stability.

## Acceptance criteria

- [x] Comparator is unit-tested for mixed complete/incomplete and equal created dates.
- [x] `done` and `cancelled` both sort after incomplete.


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
| Marco Mendão | 2026-08-28T23:07:00Z | 2026-08-28T23:07:29Z | Shared comparator + unit tests for incomplete-then-newest sort. |

