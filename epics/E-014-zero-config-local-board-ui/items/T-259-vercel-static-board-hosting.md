---
id: T-259
type: task
title: Host board package on Vercel as static site
status: done
priority: high
size: M
size_source: suggested
size_basis: [calibrated:T-259]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 4
estimate_source: suggested
estimate_basis: [calibrated:T-259]
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
tags: [vercel, static, board, deploy, init]
created: 2026-07-29
updated: 2026-07-29T07:31:14.976Z
started_at: 2026-07-29T05:47:29Z
completed_at: 2026-07-29T06:02:31Z
actual_ms: 253000
---
# T-259: Host board package on Vercel as static site

## Description

Configure `taskmark-taskmark` (and board-ui stubs from `ensure-board-ui` / `taskmark-init`) so Vercel runs a **production build** and serves the static HTML output — not Framework Preset Node + `server.js` / `npm start` serve.

## Acceptance criteria

- [x] Board `vercel.json` / project settings use a build command and static output directory (no Node `server.js` entry required for hosted boards).
- [x] `taskmark-taskmark` deploys on Vercel by building static files from the board UI + this board’s markdown.
- [x] `ensure-board-ui.py` / init stubs and README match the static deploy path (replace Node-serve docs).
- [x] Redeploy after board markdown changes refreshes the published static site.

## Notes

Depends on T-258. Replaces T-256 Node-serve hosting approach for Vercel.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 2 | 2026-07-29T05:47:29Z | prompt | Marco Mendão | implement everything you created (T-257–T-259) |
| 1 | 2026-07-29T05:40:31Z | prompt | Marco Mendão | Board on Vercel should build and serve static HTML like production |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T05:47:29Z | 2026-07-29T05:51:42Z | shared-batch: vercel.json static out/ + init stubs |
