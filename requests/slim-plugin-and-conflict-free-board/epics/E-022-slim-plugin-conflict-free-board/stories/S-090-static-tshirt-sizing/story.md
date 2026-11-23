---
id: S-090
type: story
title: Static t-shirt sizing with new points map
status: backlog
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 16
points_source: rolled_up
estimate_minutes: 160
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-022
epic: E-022
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, collaboration, board]
created: 2026-08-28
updated: 2026-08-28T12:37:43.783Z
started_at: null
completed_at: null
actual_ms: 0
---

# S-090: Static t-shirt sizing with new points map

## User story

As someone creating work, I want a fixed size→points table so that estimates do not drift from velocity calibration or SIZING.md.

## Acceptance criteria

- [ ] Create flow uses only: XS=1, S=3, M=5, L=8, XL=13, XXL=21 with the agreed meanings.
- [ ] No Current Speed / median min/pt / calibrate path writes sizes or estimates.
- [ ] UI and docs show the static table; XXL means not sprint-ready (prefer split).

## Tasks

- [T-291: Encode XS–XXL static size and points in create + conventions](items/T-291-encode-static-size-map.md)
- [T-292: Remove velocity, calibration, and speed-based estimates](items/T-292-remove-velocity-calibration.md)
- [T-293: Update docs and sample items for static sizing](items/T-293-docs-sample-static-sizing.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-28T12:19:14Z | prompt | Marco Mendão | Full housekeeping: slim commands, drop derived board files, static sizing, leaf-only MD, new IDs, delete unused plugin pieces. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
