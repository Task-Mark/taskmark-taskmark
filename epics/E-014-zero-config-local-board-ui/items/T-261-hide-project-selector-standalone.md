---
id: T-261
type: task
title: Hide project selector in standalone serve mode
status: backlog
priority: medium
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 25
actual_minutes: 0
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
resolvers: []
blocked: false
cancelled: false
tags: [frontend, ui, serve, standalone]
created: 2026-07-29
updated: 2026-07-29T06:48:27.505Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-261: Hide project selector in standalone serve mode

## Description

When the board UI runs in the standalone product mode — the user opens a board with `npx taskmark serve` (or equivalent) from inside the taskmark / board project folder — the project selector dropdown must not appear. That control is for multi-master / cookie-based workspace switching, not for a single auto-bound board.

## Acceptance criteria

- [ ] With `npx taskmark serve` (or auto-bound board from cwd/env), the project selector dropdown is not rendered.
- [ ] Multi-master / cookie-based setup that still needs project switching continues to show the selector when appropriate.
- [ ] Layout remains usable with the selector absent (no empty gap or broken chrome).

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-29T05:50:53Z | prompt | Marco Mendão | Standalone npx serve: project selector dropdown should not exist |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
