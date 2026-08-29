---
id: T-MO-56ec25df
type: task
title: Separate expand control from open-detail actions
status: done
priority: high
size: S
points: 3
parent: S-MO-6d9a5f48
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
started_at: 2026-08-28T23:15:13Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-56ec25df: Separate expand control from open-detail actions

## Description

Chevron (or equivalent) toggles expand. Title/id/view button opens the sheet or focuses the row without toggling expand unless that is the only hit target on a small row.

## Acceptance criteria

- [x] Clicking View does not toggle expand.
- [x] Clicking the chevron does not open the sheet.


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
| Marco Mendão | 2026-08-28T23:15:13Z | 2026-08-28T23:15:42Z | Separate chevron expand from View detail button. |

