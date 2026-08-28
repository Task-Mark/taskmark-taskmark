---
id: T-283
type: task
title: Delete all other slash commands
status: done
priority: high
size: M
size_source: manual
size_basis: []
points: 5
points_source: manual
estimate_minutes: 50
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:10min/pt]
session_cap_minutes: 480
parent: S-088
epic: E-022
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
tags: [plugin, collaboration, board]
created: 2026-08-28
updated: 2026-08-28T15:43:42Z
started_at: 2026-08-28T15:33:55Z
completed_at: 2026-08-28T15:43:42Z
actual_ms: 0
---
# T-283: Delete all other slash commands

## Description

Remove every command under `plugins/taskmark/commands/` except the four `tsmk-*` files. Update plugin.json / Cursor command registration.

## Acceptance criteria

- [x] No leftover `/new-epic`, `/new-story`, `/new-task`, `/start-work`, `/complete-work`, `/sync-status`, `/board-status`, `/velocity`, `/commit-all`, `/log-commits`, `/sync-repos`, `/sync-plugin-local`.
- [x] Cursor only lists the four tsmk commands for this plugin.

## Notes

Static sizing for this epic uses the new map (XS=1, S=3, M=5, L=8, XL=13, XXL=21).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-28T12:19:14Z | prompt | Marco Mendão | Arrumar a casa: four tsmk-* commands, drop INDEX/SIZING/VELOCITY/README, leaf-only writes, race-free IDs, delete unused plugin surface. |
| 2 | 2026-08-28T15:43:42Z | feedback | Marco Mendão | Implemented and verified as part of E-022; no commits created. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-08-28T15:33:55Z | 2026-08-28T15:34:19Z | E-022 shared batch: implemented and verified T-283 (5 points); no commit. |
