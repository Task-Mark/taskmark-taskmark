---
id: T-284
type: task
title: Rewrite always-apply rules for the four-command model
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
started_at: 2026-08-28T15:34:19Z
completed_at: 2026-08-28T15:43:42Z
actual_ms: 0
---
# T-284: Rewrite always-apply rules for the four-command model

## Description

Update `taskmark-project-memory` and `taskmark-conventions` rules so agents use only tsmk-* flows, leaf-only writes, static sizing, and no derived-file refresh.

## Acceptance criteria

- [x] Rules no longer mention start-work, complete-work, sync-status, INDEX, VELOCITY, README dashboard, or calibrate.
- [x] Rules state `/tsmk-do` never commits and does not use `in_progress`.

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
| 1 | Marco Mendão | 2026-08-28T15:34:19Z | 2026-08-28T15:34:58Z | E-022 shared batch: implemented and verified T-284 (8 points); no commit. |
