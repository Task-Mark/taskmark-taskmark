---
id: B-018
type: bug
title: ERR_TOO_MANY_REDIRECTS — serve the board at / instead of redirecting
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 10
actual_minutes: 9
estimate_source: suggested
estimate_basis: [calibrated:B-018]
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
tags: [frontend, routing, ui]
created: 2026-08-17
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-08-17T07:45:00Z
completed_at: 2026-08-17T07:54:20Z
actual_ms: 560000
---
# B-018: ERR_TOO_MANY_REDIRECTS — serve the board at / instead of redirecting

## Description

`/` was never a real page: it only redirected to `/board` or `/setup`, and `/setup` redirected back. Any disagreement between those three handlers — a prerendered `/setup`, a stale cookie, an older published build — produced `ERR_TOO_MANY_REDIRECTS` in the browser instead of a board.

The board is now rendered **at `/`**, and `/setup` is only reached when the workspace has no bound project (the `mode: workspace` case).

## Repro steps

1. Run the UI where no board binds and the browser has stale board cookies.
2. Open `http://localhost:8275`.
3. Browser bounces `/` → `/setup` → `/board` → `/setup` and reports `ERR_TOO_MANY_REDIRECTS`.

## Fix criteria

- [x] `/` renders the board directly in bound mode (HTTP 200, no redirect).
- [x] `/` redirects once to `/setup` only when there is no project to show (workspace mode).
- [x] `/setup` redirects to `/` (never `/board`) once a project is bound or chosen.
- [x] `/board` still returns the board so old links and bookmarks keep working.
- [x] Internal links and server actions target `/`.
- [x] Static export puts the board in `index.html`.

## Notes

Board rendering moved out of `app/board/page.tsx` into `components/board/board-screen.tsx`. Both `/` and `/board` are thin wrappers over it, so there is no redirect between them and no duplicated logic. `boardHref` and the hardcoded epic/story links now emit `/?…`; `saveMasterFolder`, `selectActiveProject`, and `openAddProject` redirect to `/`.

`app/page.tsx` joined the static build's force-dynamic → force-static swap list.

Verified with the prebuilt server. Bound (from board folder): `/` 200 board, `/board` 200, `/setup` 307 → `/`, `/?epic=E-014` 200. Workspace (from `/tmp`): `/` 307 → `/setup` 200 wizard; with a master cookie `/` 200 with project picker. `taskmark build` emits `index.html` containing the board.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-17T07:45:00Z | prompt | Marco Mendão | ERR_TOO_MANY_REDIRECTS; board should be at / and /setup only in workspace mode |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| e8cba45 | taskmark-frontend | 2026-08-17T09:56:59Z | Marco Mendão | serve board at / and keep static build out of serve |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-08-17T07:45:00Z | 2026-08-17T07:54:20Z | Board rendered at / via shared BoardScreen; /board kept as alias; setup only for workspace mode |
