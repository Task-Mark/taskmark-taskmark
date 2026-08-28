---
id: T-285
type: task
title: Stop writing INDEX.md; UI scans epics/
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
started_at: 2026-08-28T15:34:58Z
completed_at: 2026-08-28T15:43:42Z
actual_ms: 0
---
# T-285: Stop writing INDEX.md; UI scans epics/

## Description

Remove INDEX generation from recompute/init/skills. Frontend (and serve) builds the board index by walking epic/story/task markdown.

## Acceptance criteria

- [x] INDEX.md is not created or updated by the plugin.
- [x] Local board UI still shows epics, stories, and tasks.
- [x] Existing INDEX.md can be deleted from the board repo and gitignored or simply not regenerated.

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
| 1 | Marco Mendão | 2026-08-28T15:34:58Z | 2026-08-28T15:35:37Z | E-022 shared batch: implemented and verified T-285 (8 points); no commit. |
