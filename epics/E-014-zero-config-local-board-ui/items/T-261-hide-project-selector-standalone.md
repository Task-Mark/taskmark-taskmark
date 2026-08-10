---
id: T-261
type: task
title: Hide project selector in standalone serve mode
status: done
priority: medium
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 25
actual_minutes: 2
estimate_source: suggested
estimate_basis: [speed:90d:13min/pt]
session_cap_minutes: 480
parent: E-014
epic: E-014
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [frontend, ui, serve, standalone]
created: 2026-07-29
updated: 2026-07-29T11:30:07.936Z
started_at: 2026-07-29T07:08:36Z
completed_at: 2026-07-29T07:13:00Z
actual_ms: 120000
---
# T-261: Hide project selector in standalone serve mode

## Description

When the board UI runs in the standalone product mode — the user opens a board with `npx taskmark serve` (or equivalent) from inside the taskmark / board project folder — the project selector dropdown must not appear. That control is for multi-master / cookie-based workspace switching, not for a single auto-bound board.

## Acceptance criteria

- [x] With `npx taskmark serve` (or auto-bound board from cwd/env), the project selector dropdown is not rendered.
- [x] Multi-master / cookie-based setup that still needs project switching continues to show the selector when appropriate.
- [x] Layout remains usable with the selector absent (no empty gap or broken chrome).

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-29T05:50:53Z | prompt | Marco Mendão | Standalone npx serve: project selector dropdown should not exist |
| 2 | 2026-07-29T07:08:36Z | prompt | Marco Mendão | implement T-260, T-261 and T-262 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T07:08:36Z | 2026-07-29T07:10:36Z | shared-batch: 1 of 4min by points — Hide project selector when autoconfig/serve-bound |
