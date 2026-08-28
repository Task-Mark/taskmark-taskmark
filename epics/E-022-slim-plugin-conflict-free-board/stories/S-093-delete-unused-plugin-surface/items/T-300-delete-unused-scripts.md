---
id: T-300
type: task
title: Delete unused plugin scripts
status: done
priority: high
size: L
size_source: manual
size_basis: []
points: 8
points_source: manual
estimate_minutes: 80
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:10min/pt]
session_cap_minutes: 480
parent: S-093
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
started_at: 2026-08-28T15:42:39Z
completed_at: 2026-08-28T15:43:42Z
actual_ms: 0
---
# T-300: Delete unused plugin scripts

## Description

Remove refresh-readme-dashboard, upsert-readme-contributors (if unused), INDEX/VELOCITY writers, calibrate, and any script only referenced by deleted skills. Keep git-identity, ensure-general-epic, sync-taskmark-repos, commit-all-repos, ensure-board-ui as needed.

## Acceptance criteria

- [x] Dead scripts are gone from plugins/taskmark/scripts.
- [x] Remaining scripts are referenced by tsmk-* or init.
- [x] recompute-actuals is removed or slimmed so it does not rewrite parents/INDEX/README/VELOCITY.

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
| 1 | Marco Mendão | 2026-08-28T15:42:39Z | 2026-08-28T15:43:18Z | E-022 shared batch: implemented and verified T-300 (8 points); no commit. |
