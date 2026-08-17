---
id: B-010
type: bug
title: "taskmark build --board . resolves against UI package cwd"
status: done
priority: high
size: XS
size_source: suggested
size_basis: []
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 1
estimate_source: suggested
estimate_basis: [speed:90d:14min/pt]
session_cap_minutes: 480
parent: E-014
epic: E-014
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
tags: [cli, build, static, packaging]
created: 2026-07-29
updated: 2026-08-17T08:03:41.619Z
started_at: 2026-07-29T06:15:52Z
completed_at: 2026-07-29T06:17:00Z
actual_ms: 68000
---
# B-010: taskmark build --board . resolves against UI package cwd

## Description

`taskmark build` spawns `build-static.mjs` with `cwd` = `@taskmark/ui` package root. Relative `--board .` / `--out out` then resolve inside `node_modules/@taskmark/ui`, so board detection fails with “No Taskmark board found”.

## Repro steps

1. From `taskmark-taskmark`: `yarn build` / `npm run build` (`taskmark build --board . --out out`).
2. Error: No Taskmark board found.

## Fix criteria

- [x] Relative `--board` / `--out` resolve against caller cwd (`INIT_CWD` / invoke cwd), not the UI package root.
- [x] `npm run build` from a board root succeeds without requiring an absolute path.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|-----| d220a7b | taskmark-frontend | 2026-07-29T06:51:55Z | Marco Mendão | add static board build and preview |
| 81dda43 | taskmark-cursor | 2026-07-29T06:51:55Z | Marco Mendão | add board preview and static hosting stubs |
| 6f9db22 | taskmark-taskmark | 2026-07-29T06:51:56Z | Marco Mendão | sync taskmark board |
-------|------|--------|---------|
| 1 | 2026-07-29T06:15:52Z | prompt | Marco Mendão | fix taskmark build --board . cwd bug |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T06:15:52Z | 2026-07-29T06:17:00Z | Resolve --board/--out against INIT_CWD; bump 0.2.1 |
