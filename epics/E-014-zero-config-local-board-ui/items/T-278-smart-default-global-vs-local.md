---
id: T-278
type: task
title: Smart default — global setup vs local board bind
status: done
priority: high
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 24
actual_minutes: 1
estimate_source: suggested
estimate_basis: [speed:90d:12min/pt]
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
tags: [frontend, cli, workspace, packaging]
created: 2026-08-14
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-08-14T17:49:09Z
completed_at: 2026-08-14T17:50:33Z
actual_ms: 84000
---

# T-278: Smart default — global setup vs local board bind

## Description

Bare `taskmark` / `npx @taskmark/ui` should pick the right mode from context:

- **Global / no local board** → standalone workspace UI with the setup / project picker.
- **Inside a Taskmark project** (board root, nested `./taskmark/`, or sibling `*-taskmark`) → bind to that board and skip setup.

`open` stays force-workspace; `serve` / `dev` stay force-bound (unless `--workspace`).

## Acceptance criteria

- [x] Bare `taskmark` with no board nearby starts workspace mode (setup wizard).
- [x] Bare `taskmark` from a board folder or product with a resolvable board binds to that board.
- [x] `taskmark open` always forces workspace mode.
- [x] `taskmark serve` / `dev` still require a board (or `--workspace`).
- [x] Help and README describe the smart default.

## Notes

Default command is internal `auto`: resolve board → bound `serve`, else workspace. Verified from `/tmp` (workspace), `taskmark-taskmark` (cwd), `taskmark-frontend` (sibling), and `open` inside a board (forced workspace).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-14T17:49:09Z | prompt | Marco Mendão | Global npx @taskmark/ui → setup flow; run inside a taskmark project → bind local board |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 51b972b | taskmark-frontend | 2026-08-14T17:52:38Z | Marco Mendão | add smart workspace and local board launch |
| 4f027b0 | taskmark-taskmark | 2026-08-14T17:52:41Z | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-08-14T17:49:09Z | 2026-08-14T17:50:33Z | Smart default auto: bind when board resolvable, else workspace; README/help updated |
