---
id: T-MO-34f59ba6
type: task
title: Keyboard and ARIA for Overall expand
status: done
priority: high
size: M
points: 5
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
started_at: 2026-08-28T23:16:11Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-34f59ba6: Keyboard and ARIA for Overall expand

## Description

Expand controls are keyboard operable (Enter/Space). Expose `aria-expanded` and a coherent tree or treegrid structure so screen readers can follow parent/child.

## Acceptance criteria

- [x] Focused expand control toggles with keyboard.
- [x] `aria-expanded` reflects state.
- [x] Nested rows are announced as related to their parent (tree/treegrid or equivalent).


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
| Marco Mendão | 2026-08-28T23:16:11Z | 2026-08-28T23:16:40Z | Enter/Space expand and aria-expanded tree roles. |

