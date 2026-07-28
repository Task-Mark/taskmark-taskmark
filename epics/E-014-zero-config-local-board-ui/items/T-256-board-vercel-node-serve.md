---
id: T-256
type: task
title: Make board package Vercel-deployable via Node serve
status: in_progress
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 230
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
resolvers: []
blocked: false
cancelled: false
tags: [deploy, vercel, board, serve]
created: 2026-07-28
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-28T15:23:18Z
completed_at: null
actual_ms: 13814846
---
# T-256: Make board package Vercel-deployable via Node serve

## Description

Configure the Taskmark board folder (`taskmark-taskmark` / board stub) so it can be deployed on Vercel by selecting the **Node** framework preset and running the `taskmark serve` entry (root `server.js` + `npm start`).

## Acceptance criteria

- [x] Board root has a Vercel-detectable Node entry (`server.js`) that starts the UI with `TASKMARK_BOARD` bound to the deployment root.
- [x] `package.json` install works on Vercel (registry `@taskmark/ui`, not sibling `file:`).
- [x] `npm start` / serve scripts run without opening a browser in hosted environments.
- [x] Board markdown is included in the deploy; README documents Vercel Node setup.
- [x] `taskmark-init` (and create-* / sync when bootstrapping) always runs `ensure-board-ui.py` so Vercel Node stubs are present.

## Notes

`ensure-board-ui.py` is Taskmark’s Vercel init — do not run CLI `vercel init` (downloads unrelated examples).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-28T15:23:18Z | prompt | Marco Mendão | Make taskmark folder runnable on Vercel as Node project running serve |
| 2 | 2026-07-28T15:32:11Z | prompt | Marco Mendão | Run Vercel init during /taskmark-init and other board bootstrap commands |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| ab9106c | taskmark-cursor | 2026-07-28T15:34:40Z | Marco Mendão | add ensure-board-ui vercel stubs on init |
| 0922bae | taskmark-frontend | 2026-07-28T15:34:40Z | Marco Mendão | skip browser open on hosted serve |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T15:23:18Z | — | In progress: Vercel Node serve for board package |
