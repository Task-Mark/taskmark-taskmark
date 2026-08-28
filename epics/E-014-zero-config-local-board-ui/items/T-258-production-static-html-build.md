---
id: T-258
type: task
title: Add production static HTML build for board UI
status: done
priority: high
size: L
size_source: suggested
size_basis: [calibrated:T-258]
points: 5
points_source: suggested
estimate_minutes: 10
actual_minutes: 7
estimate_source: suggested
estimate_basis: [calibrated:T-258]
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
tags: [frontend, build, static, vercel, packaging]
created: 2026-07-29
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-07-29T05:47:29Z
completed_at: 2026-07-29T06:02:31Z
actual_ms: 422000
---
# T-258: Add production static HTML build for board UI

## Description

Stop treating hosted board UI as `npm run serve` / Node standalone only. Add a **production build** that emits static HTML (and assets) suitable for Vercel static hosting — a real `next build` (or equivalent static export) of the board UI bound to the board markdown at build time.

## Acceptance criteria

- [x] Board UI / board package has a build command that produces static HTML + assets (not only a long-running `taskmark serve`).
- [x] Build can target a board root (`TASKMARK_BOARD` / cwd) so pages reflect that board’s content.
- [x] Output is self-contained enough to serve without a Node server process.
- [x] Local `taskmark serve` for interactive board editing remains supported (build path is additive for hosted/static).

## Notes

Supersedes the hosted direction of T-256 (Node `server.js` serve) for Vercel. Interactive local CLI serve can stay.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 2 | 2026-07-29T05:47:29Z | prompt | Marco Mendão | implement everything you created (T-257–T-259) |
| 1 | 2026-07-29T05:40:31Z | prompt | Marco Mendão | Board on Vercel should build static HTML, not npm run serve |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T05:47:29Z | 2026-07-29T05:54:31Z | shared-batch: taskmark build static HTML snapshot export |
