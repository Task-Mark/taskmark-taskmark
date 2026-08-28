---
id: T-292
type: task
title: Remove velocity, calibration, and speed-based estimates
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
parent: S-090
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
started_at: 2026-08-28T15:37:43Z
completed_at: 2026-08-28T15:43:42Z
actual_ms: 0
---
# T-292: Remove velocity, calibration, and speed-based estimates

## Description

Drop recompute --calibrate, VELOCITY metrics as a board file, estimate_basis speed:90d, and UI Current Speed if it depended on VELOCITY.md. Estimate minutes may be 0 or unused.

## Acceptance criteria

- [x] No script updates historical done-item sizes from actuals.
- [x] Create does not set estimate from 90-day median.
- [x] Board UI does not require VELOCITY.md.

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
| 1 | Marco Mendão | 2026-08-28T15:37:43Z | 2026-08-28T15:38:22Z | E-022 shared batch: implemented and verified T-292 (8 points); no commit. |
