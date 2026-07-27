---
id: T-178
type: task
title: Remove velocity and estimate calibration from recompute
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 2
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-057
epic: E-015
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
tags: [plugin, velocity, shelved]
created: 2026-07-27
updated: 2026-07-27T06:17:22.249Z
started_at: 2026-07-27T06:10:41Z
completed_at: 2026-07-27T06:17:22Z
actual_ms: 120000
---
# T-178: Remove velocity and estimate calibration from recompute

## Description

Strip median min/point, VELOCITY refresh, and estimate calibration/suggestion from `recompute-actuals.py`.

## Acceptance criteria

- [x] `--calibrate` does not rewrite open non-manual estimates from 30-day median min/point.
- [x] Script documents that velocity estimate refresh is shelved.
- [x] Actual minutes, rollups, and INDEX updates still work.


## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T06:10:25Z | prompt | Marco Mendão | Shelf velocity docs and estimate mechanism for now; reimplement later |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:12:41Z | 2026-07-27T06:14:41Z | shared-batch: 2 of 6min by points — remove velocity (T-178) |
