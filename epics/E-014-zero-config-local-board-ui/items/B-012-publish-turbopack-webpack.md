---
id: B-012
type: bug
title: "npm publish prepack fails: Turbopack vs webpack config"
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
tags: [packaging, next, publish]
created: 2026-07-29
updated: 2026-07-29T07:31:14.976Z
started_at: 2026-07-29T06:32:00Z
completed_at: 2026-07-29T06:33:57Z
actual_ms: 117000
---
# B-012: npm publish prepack fails: Turbopack vs webpack config

## Description

`npm publish` runs `prepack` → `next build`. Next 16 defaults to Turbopack, but `next.config.ts` defines `webpack` (for `@/` alias) without a turbopack config, so the build errors and publish aborts.

## Repro steps

1. In `taskmark-frontend`: `npm publish` (or `npm run build`).
2. Error: Turbopack with webpack config and no turbopack config.

## Fix criteria

- [x] `npm run build` / prepack completes with standalone output.
- [x] Explicit webpack (or turbopack alias parity) so Next 16 does not reject the config.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|-----| d220a7b | taskmark-frontend | 2026-07-29T06:51:55Z | Marco Mendão | add static board build and preview |
| 81dda43 | taskmark-cursor | 2026-07-29T06:51:55Z | Marco Mendão | add board preview and static hosting stubs |
| 6f9db22 | taskmark-taskmark | 2026-07-29T06:51:56Z | Marco Mendão | sync taskmark board |
-------|------|--------|---------|
| 1 | 2026-07-29T06:32:00Z | prompt | Marco Mendão | npm publish prepack fails on Turbopack vs webpack |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T06:32:00Z | 2026-07-29T06:33:57Z | next build --webpack; turbopack resolveAlias for @ |
