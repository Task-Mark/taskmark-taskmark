---
id: T-280
type: task
title: Add /tsmk-create for epic, story, task, or tree
status: done
priority: high
size: XL
size_source: manual
size_basis: []
points: 13
points_source: manual
estimate_minutes: 130
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
started_at: 2026-08-28T15:31:34Z
completed_at: 2026-08-28T15:43:42Z
actual_ms: 0
---
# T-280: Add /tsmk-create for epic, story, task, or tree

## Description

One create command: user names type or pastes a description; agent creates epic and/or stories and/or tasks. Create must write only new item files (no parent Tasks lists or rollups) per S-091.

## Acceptance criteria

- [x] Can create a single epic, story, or task/bug.
- [x] Can create an epic plus nested stories and tasks from one description.
- [x] Does not edit parent markdown lists or INDEX/README/SIZING/VELOCITY.

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
| 1 | Marco Mendão | 2026-08-28T15:31:34Z | 2026-08-28T15:32:37Z | E-022 shared batch: implemented and verified T-280 (13 points); no commit. |
