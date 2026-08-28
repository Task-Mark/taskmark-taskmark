---
id: T-MO-a8de0ef8
type: task
title: Rename slash commands from tsmk to tkmd
status: done
priority: high
size: S
points: 3
parent: S-088
epic: E-022
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
tags: [plugin, commands]
created: 2026-08-28
updated: 2026-08-28T23:00:00Z
started_at: 2026-08-28T22:53:17Z
completed_at: 2026-08-28T23:00:00Z
---

# T-MO-a8de0ef8: Rename slash commands from tsmk to tkmd

## Description

User-facing Cursor commands must be `/tkmd-init`, `/tkmd-create`, `/tkmd-do`,
and `/tkmd-commit` instead of `/tsmk-*`.

## Acceptance criteria

- [x] Plugin command files are `tkmd-init`, `tkmd-create`, `tkmd-do`, `tkmd-commit`.
- [x] Matching create/do skills use the `tkmd-` names.
- [x] Rules, plugin README, website, and landing demo use `/tkmd-*`.
- [x] Plugin tests pass and the local plugin is synced.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-28T22:52:00Z | prompt | Marco Mendão | em vez dos comandos terem o prefixo /tsmk-comando deveram ter /tkmd-comando altera isto |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-28T22:53:17Z | 2026-08-28T23:00:00Z | Renamed Cursor commands and create/do skills from tsmk to tkmd; updated docs and plugin tests. |
