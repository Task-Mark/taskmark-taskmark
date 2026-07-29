---
id: B-011
type: bug
title: "taskmark build snapshot fails on @/ path aliases under tsx"
status: done
priority: high
size: XS
size_source: suggested
size_basis: [calibrated:B-011]
points: 1
points_source: suggested
estimate_minutes: 10
actual_minutes: 11
estimate_source: suggested
estimate_basis: [calibrated:B-011]
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
updated: 2026-07-29T06:48:27.505Z
started_at: 2026-07-29T06:20:00Z
completed_at: 2026-07-29T06:31:30Z
actual_ms: 690000
---
# B-011: taskmark build snapshot fails on @/ path aliases under tsx

## Description

After board path resolution (B-010), `taskmark build` fails writing `public/taskmark-snapshot.json` because `tsx` cannot resolve `@/` imports from `lib/taskmark/build-snapshot.ts` when the package lives under `node_modules/@taskmark/ui`.

## Repro steps

1. From a board with `@taskmark/ui` installed: `yarn build` / `npm run build`.
2. Error: `Cannot find package '@/lib' imported from .../build-snapshot.ts`.

## Fix criteria

- [x] Snapshot step resolves `@/` (or avoids aliases) when run from an installed package.
- [x] Full `taskmark build --board . --out out` produces a static `out/` site.

## Notes

Bundle `write-board-snapshot.ts` with esbuild (`alias: { "@": packageRoot }`) then run the ESM bundle with Node. Stage the UI to `<board>/.taskmark-ui-build` when the package lives under `node_modules` (Next won't transpile TS there). Pin Next `outputFileTracingRoot` / webpack `@` alias; ship `typescript` + `@types/*` as runtime deps so staged builds skip Next's auto-install.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|-----| d220a7b | taskmark-frontend | 2026-07-29T06:51:55Z | Marco Mendão | add static board build and preview |
| 81dda43 | taskmark-cursor | 2026-07-29T06:51:55Z | Marco Mendão | add board preview and static hosting stubs |
| 6f9db22 | taskmark-taskmark | 2026-07-29T06:51:56Z | Marco Mendão | sync taskmark board |
-------|------|--------|---------|
| 1 | 2026-07-29T06:20:00Z | prompt | Marco Mendão | terminal error: Cannot find package '@/lib' during taskmark build snapshot |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T06:20:00Z | 2026-07-29T06:31:30Z | esbuild snapshot bundle; stage UI outside node_modules; Next root/alias; typescript as dep |
