---
id: B-009
type: bug
title: "@taskmark/ui must be a production dependency for Vercel"
status: done
priority: high
size: M
size_source: suggested
size_basis: [calibrated:B-009]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 7
estimate_source: suggested
estimate_basis: [calibrated:B-009]
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
tags: [vercel, npm, packaging, board]
created: 2026-07-28
updated: 2026-08-17T08:03:41.619Z
started_at: 2026-07-28T19:06:10Z
completed_at: 2026-07-28T19:13:32Z
actual_ms: 442000
---

# B-009: @taskmark/ui must be a production dependency for Vercel

## Description

Vercel production installs omit `devDependencies`. If `@taskmark/ui` is installed with `--save-dev`, the board `server.js` entry cannot resolve `dist/standalone/server.js` at deploy time (`/var/task/node_modules/@taskmark/ui/...` missing).

## Repro steps

1. Board `package.json` has `@taskmark/ui` only under `devDependencies` (or init used `npm i -D`).
2. Deploy board repo to Vercel (Framework Preset: Node, `server.js`).
3. Runtime fails: standalone server missing under `@taskmark/ui`.

## Fix criteria

- [x] `vercel.json` `functions.server.js.includeFiles` covers `@taskmark/ui` + board markdown (NFT).
- [x] Board `server.js` uses literal `require.resolve('@taskmark/ui/dist/standalone/server.js')`.
- [x] Board `package.json` keeps `@taskmark/ui` under `dependencies` (not `devDependencies`).
- [x] `ensure-board-ui.py` always migrates `@taskmark/ui` out of `devDependencies` into `dependencies`.
- [x] `taskmark-init` / docs / CLI help install with `--save` (never `-D` / `--save-dev`).
- [x] Frontend README and `taskmark` help examples use production install.

## Notes

Related: T-256 (Vercel Node serve stubs).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-28T19:06:10Z | prompt | Marco Mendão | Vercel missing standalone server; keep @taskmark/ui out of devDependencies |
| 2 | 2026-07-28T19:08:00Z | note | Marco Mendão | Also fixed vercel.json includeFiles + static require.resolve for NFT |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 5615050 | taskmark-taskmark | 2026-07-28T19:13:43Z | Marco Mendão | fix B-009 vercel ui production dep |
| e2b0fda | taskmark-frontend | 2026-07-28T19:13:32Z | Marco Mendão | document @taskmark/ui as production dependency |
| 62f8af2 | taskmark-cursor | 2026-07-28T19:13:32Z | Marco Mendão | keep @taskmark/ui as production dep on vercel |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T19:06:10Z | 2026-07-28T19:13:32Z | @taskmark/ui production dep; vercel includeFiles; docs --save |
