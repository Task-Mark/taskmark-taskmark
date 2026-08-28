---
id: T-296
type: task
title: Derive parent lists, status, and rollups in the UI
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
parent: S-091
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
started_at: 2026-08-28T15:39:54Z
completed_at: 2026-08-28T15:43:42Z
actual_ms: 0
---
# T-296: Derive parent lists, status, and rollups in the UI

## Description

Board UI (and any in-memory index) aggregates children by parent/epic fields. Do not persist rollups into parent markdown.

## Acceptance criteria

- [x] Epic/story detail lists children by scanning files.
- [x] Displayed points/status for parents are computed at read time.
- [x] No plugin step is required to refresh parent files after leaf edits.

## Notes

Static sizing for this epic uses the new map (XS=1, S=3, M=5, L=8, XL=13, XXL=21).

UI hoje: listas leem frontmatter; filhos vêm de pastas + `attachChildren` em `detail-load.ts`; pontos/status do pai não são derivados em read-time (só `count-leaves.ts` para progresso). Logs/pessoas/datas do pai ficam em [T-302](T-302-parent-ui-from-leaf-logs-status-people-dates.md).

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
| 1 | Marco Mendão | 2026-08-28T15:39:54Z | 2026-08-28T15:40:33Z | E-022 shared batch: implemented and verified T-296 (8 points); no commit. |
