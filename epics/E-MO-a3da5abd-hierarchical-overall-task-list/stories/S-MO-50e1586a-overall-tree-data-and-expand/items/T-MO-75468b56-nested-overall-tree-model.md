---
id: T-MO-75468b56
type: task
title: Nested Overall tree types and parser
status: done
priority: high
size: L
points: 8
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
started_at: 2026-08-28T23:07:29Z
completed_at: 2026-08-28T23:17:07Z
---

# T-MO-75468b56: Nested Overall tree types and parser

## Description

Introduce a nested tree type (epic nodes with story/item children; story nodes with task/bug children) built from the existing board index/parsers. Do not require stacked parse-on-select tables.

## Acceptance criteria

- [x] One structure can render the full Overall hierarchy for a project.
- [x] Epic-direct items are first-class children of the epic node.
- [x] Parse errors still surface without dropping the rest of the tree.


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
| Marco Mendão | 2026-08-28T23:07:29Z | 2026-08-28T23:07:58Z | Nested Overall tree types and builder from existing parsers. |

