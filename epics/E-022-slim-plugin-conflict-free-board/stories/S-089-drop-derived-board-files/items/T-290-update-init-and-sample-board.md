---
id: T-290
type: task
title: Update init and sample board to the new file set
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
parent: S-089
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
started_at: 2026-08-28T15:36:55Z
completed_at: 2026-08-28T15:43:42Z
actual_ms: 0
---
# T-290: Update init and sample board to the new file set

## Description

taskmark-init, examples/sample-board, and ensure-board-ui must not seed removed files; keep epics/ + UI stubs.

## Acceptance criteria

- [x] New boards have no INDEX/SIZING/VELOCITY/README/committed REPOS.
- [x] Sample board in the plugin repo matches.
- [x] Serve/build still works.

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
| 1 | Marco Mendão | 2026-08-28T15:36:55Z | 2026-08-28T15:37:19Z | E-022 shared batch: implemented and verified T-290 (5 points); no commit. |
