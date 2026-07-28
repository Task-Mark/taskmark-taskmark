---
id: E-014
type: epic
title: Zero-config local board UI package
status: in_progress
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 39
points_source: rolled_up
estimate_minutes: 400
actual_minutes: 260
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
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
tags: [frontend, packaging, cli, npm, local, vercel]
created: 2026-07-24
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-28T08:09:03Z
completed_at: null
actual_ms: 15618846
---

# E-014: Zero-config local board UI package

## Goal

Ship Taskmark’s web UI so a developer can open a local board with `npx taskmark serve` (default port **8275**) — no cloning `taskmark-frontend`, no setup wizard, and no manual path configuration when the board is already on disk.

## Scope

- Auto-bind the UI to a board from env (`TASKMARK_BOARD` / `TASKMARK_MASTER`) or cwd (nested `taskmark/` or flat `*-taskmark` root).
- Skip `/setup` when auto-config is valid; open straight on `/board`.
- Publish an npm package with bin `taskmark` and subcommand `serve` that starts a prebuilt server against the resolved board on port **8275** by default.
- Document (and optionally scaffold) a one-command launch path when a board is created/initialized.

## Out of scope

- Docker images and static/nginx-only hosting (later).
- Hosted/cloud board sync or multi-tenant SaaS.
- Changing board markdown schema beyond what the current UI already reads.

## Success metrics

- From a product repo with `./taskmark/` (or a dedicated board root), `npx taskmark serve` opens the dashboard at `http://localhost:8275` on that board with no setup steps.
- Cookie-based multi-master setup still works when no auto-config is present.

## Stories

- [S-050: Zero-config board binding from env and cwd](stories/S-050-zero-config-board-binding/story.md)
- [S-051: Publishable npm CLI for local board UI](stories/S-051-publishable-npm-cli/story.md)
- [S-052: Board init one-command UI launch](stories/S-052-board-init-one-command-ui/story.md)

## Tasks

- [T-256: Make board package Vercel-deployable via Node serve](items/T-256-board-vercel-node-serve.md)
- [B-009: @taskmark/ui must be a production dependency for Vercel](items/B-009-ui-must-be-production-dep.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| e2b0fda | taskmark-frontend | 2026-07-28T19:13:32Z | Marco Mendão | document @taskmark/ui as production dependency |
| 62f8af2 | taskmark-cursor | 2026-07-28T19:13:32Z | Marco Mendão | keep @taskmark/ui as production dep on vercel |
| ab9106c | taskmark-cursor | 2026-07-28T15:34:40Z | Marco Mendão | add ensure-board-ui vercel stubs on init |
| 0922bae | taskmark-frontend | 2026-07-28T15:34:40Z | Marco Mendão | skip browser open on hosted serve |
| 3a3ef93 | taskmark-taskmark | 2026-07-28T14:35:04Z | Marco Mendão | log T-242 init ui install commits |
| fd924c0 | taskmark-cursor | 2026-07-28T14:34:41Z | Marco Mendão | install @taskmark/ui during taskmark-init |
| 082f140 | taskmark-taskmark | 2026-07-28T14:34:41Z | Marco Mendão | sync taskmark board |
| 31800fc | taskmark-taskmark | 2026-07-28T09:13:02Z | Marco Mendão | log T-241 @taskmark/ui commits |
| b62a48c | taskmark-frontend | 2026-07-28T09:12:29Z | Marco Mendão | publish local ui as @taskmark/ui |
| bce55d8 | taskmark-cursor | 2026-07-28T09:12:29Z | Marco Mendão | point board init at @taskmark/ui |
| bd0fede | taskmark-taskmark | 2026-07-28T09:12:29Z | Marco Mendão | sync taskmark board |
| 4d10e86 | taskmark-taskmark | 2026-07-28T08:51:45Z | Marco Mendão | log E-014 and E-019 commits |
| f9b7f3f | taskmark-frontend | 2026-07-28T09:50:48Z | Marco Mendão | add taskmark serve cli and zero-config board bind |
| d07e536 | taskmark-cursor | 2026-07-28T09:50:48Z | Marco Mendão | document taskmark serve on board init |
| 935c164 | taskmark-taskmark | 2026-07-28T09:50:56Z | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T08:31:48Z | 2026-07-28T08:31:48Z | Rollup: E-014 complete; billable on leaves (shared-batch); 0-min parent |
| 2 | Marco Mendão | 2026-07-28T14:33:38Z | 2026-07-28T14:33:38Z | Rollup: T-242 done; 0-min parent |
