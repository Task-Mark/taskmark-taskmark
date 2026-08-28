---
id: T-281
type: task
title: Add /tsmk-commit for multi-repo commits
status: done
priority: high
size: S
size_source: manual
size_basis: []
points: 3
points_source: manual
estimate_minutes: 30
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
started_at: 2026-08-28T15:32:37Z
completed_at: 2026-08-28T15:43:42Z
actual_ms: 0
---
# T-281: Add /tsmk-commit for multi-repo commits

## Description

Port commit-all behavior to `/tsmk-commit`. Keep one-line messages, no push unless asked. Must stay fully separate from `/tsmk-do`.

## Acceptance criteria

- [x] Commits every linked dirty git root with a simple message.
- [x] Does not push unless the user asks.
- [x] Is not invoked by `/tsmk-do`.

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
| 1 | Marco Mendão | 2026-08-28T15:32:37Z | 2026-08-28T15:32:52Z | E-022 shared batch: implemented and verified T-281 (3 points); no commit. |
