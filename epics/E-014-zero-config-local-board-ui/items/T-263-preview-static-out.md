---
id: T-263
type: task
title: "Add package.json preview script to serve static out/"
status: done
priority: medium
size: M
size_source: suggested
size_basis: [calibrated:T-263]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 3
estimate_source: suggested
estimate_basis: [calibrated:T-263]
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
tags: [cli, static, packaging]
created: 2026-07-29
updated: 2026-07-29T06:48:27.505Z
started_at: 2026-07-29T06:44:50Z
completed_at: 2026-07-29T06:48:27Z
actual_ms: 217000
---

# T-263: Add package.json preview script to serve static out/

## Description

After `taskmark build`, boards need a local way to preview the static `out/` site (distinct from `taskmark serve`, which runs the Next standalone server).

## Acceptance criteria

- [x] Board `package.json` (and init stub) include a `preview` script that serves `out/`.
- [x] `@taskmark/ui` exposes `taskmark preview` (port/board/out flags) without extra npm deps.
- [x] Missing `out/` prints a clear hint to run `taskmark build` first.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-29T06:44:50Z | prompt | Marco Mendão | add a command to serve the static html files in package.json |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| d220a7b | taskmark-frontend | 2026-07-29T06:51:55Z | Marco Mendão | add static board build and preview |
| 81dda43 | taskmark-cursor | 2026-07-29T06:51:55Z | Marco Mendão | add board preview and static hosting stubs |
| 6f9db22 | taskmark-taskmark | 2026-07-29T06:51:56Z | Marco Mendão | sync taskmark board |
| 64ac5d0 | taskmark-taskmark | 2026-07-29T06:52:10Z | Marco Mendão | log static build commits |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T06:44:50Z | 2026-07-29T06:48:27Z | taskmark preview CLI + package.json preview script |
