---
id: T-282
type: task
title: Add /tsmk-do implement without commit or in_progress
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
started_at: 2026-08-28T15:32:52Z
completed_at: 2026-08-28T15:43:42Z
actual_ms: 0
---
# T-282: Add /tsmk-do implement without commit or in_progress

## Description

`/tsmk-do` implements the named epic/story/task. Never commit. Do not set status to `in_progress` (avoid extra sync tokens). When the agent finishes, every leaf it executed is `done` (AC checked, `completed_at` set) on that leaf file only.

## Acceptance criteria

- [x] Never runs git commit, commit-all, or push.
- [x] Does not transition items through `in_progress`.
- [x] Executed tasks/bugs (and a story/epic only if it was the work target with no remaining open children) are `done` when the agent stops.
- [x] Only the implemented leaf markdown files are modified.

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
| 1 | Marco Mendão | 2026-08-28T15:32:52Z | 2026-08-28T15:33:55Z | E-022 shared batch: implemented and verified T-282 (13 points); no commit. |
