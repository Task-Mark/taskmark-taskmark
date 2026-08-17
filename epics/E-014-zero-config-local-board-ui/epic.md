---
id: E-014
type: epic
title: Zero-config local board UI package
status: in_progress
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 82
points_source: rolled_up
estimate_minutes: 656
actual_minutes: 1064
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
updated: 2026-08-17T08:03:41.619Z
started_at: 2026-07-28T08:09:03Z
completed_at: null
actual_ms: 63855000
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

- Docker / custom nginx images (Vercel static hosting is in scope via T-258–T-259).
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
- [T-258: Add production static HTML build for board UI](items/T-258-production-static-html-build.md)
- [T-259: Host board package on Vercel as static site](items/T-259-vercel-static-board-hosting.md)
- [B-010: taskmark build --board . resolves against UI package cwd](items/B-010-build-board-relative-cwd.md)
- [B-011: taskmark build snapshot fails on @/ path aliases under tsx](items/B-011-build-snapshot-path-aliases.md)
- [B-012: npm publish prepack fails: Turbopack vs webpack config](items/B-012-publish-turbopack-webpack.md)
- [B-013: Static build CSS warnings from `first-child` arbitrary variant Tailwind class](items/B-013-css-first-child-lightning-warnings.md)
- [T-260: Replace logo subtitle with product memory tagline](items/T-260-logo-tagline-product-memory.md)
- [T-261: Hide project selector in standalone serve mode](items/T-261-hide-project-selector-standalone.md)
- [T-262: Remove folder path references from board UI](items/T-262-remove-folder-paths-from-ui.md)
- [T-263: Add package.json preview script to serve static out/](items/T-263-preview-static-out.md)
- [B-015: taskmark serve fails: Cannot find module './cpu-profile'](items/B-015-serve-missing-cpu-profile.md)
- [T-276: Add taskmark dev with board markdown live reload](items/T-276-taskmark-dev-md-reload.md)
- [B-016: taskmark dev from product repo misses sibling *-taskmark board](items/B-016-dev-misses-sibling-taskmark-board.md)
- [T-277: Global taskmark workspace mode with project picker](items/T-277-workspace-mode-project-picker.md)
- [T-278: Smart default — global setup vs local board bind](items/T-278-smart-default-global-vs-local.md)
- [B-017: npx taskmark runs an unrelated npm package instead of the board UI](items/B-017-npx-taskmark-wrong-package.md)
- [B-018: ERR_TOO_MANY_REDIRECTS — serve the board at / instead of redirecting](items/B-018-board-at-root-redirect-loop.md)
- [B-019: taskmark build leaves a static .next that serve then runs instead of the app](items/B-019-static-build-clobbers-serve.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 51b972b | taskmark-frontend | 2026-08-14T17:52:38Z | Marco Mendão | add smart workspace and local board launch |
| 4f027b0 | taskmark-taskmark | 2026-08-14T17:52:41Z | Marco Mendão | sync taskmark board |
| bd7d5b4 | taskmark-frontend | 2026-08-10T17:04:19+01:00 | Marco Mendão | resolve sibling taskmark board from product cwd |
| 61a5097 | taskmark-taskmark | 2026-08-10T16:09:57+01:00 | Marco Mendão | sync taskmark board |
| 4db830e | taskmark-frontend | 2026-08-10T15:09:00Z | Marco Mendão | fix serve packaging and add taskmark dev |
| ac89ac0 | taskmark-cursor | 2026-08-10T15:09:00Z | Marco Mendão | point board stub dev at taskmark dev |
| d220a7b | taskmark-frontend | 2026-07-29T06:51:55Z | Marco Mendão | add static board build and preview |
| 81dda43 | taskmark-cursor | 2026-07-29T06:51:55Z | Marco Mendão | add board preview and static hosting stubs |
| 6f9db22 | taskmark-taskmark | 2026-07-29T06:51:56Z | Marco Mendão | sync taskmark board |
| 5615050 | taskmark-taskmark | 2026-07-28T19:13:43Z | Marco Mendão | fix B-009 vercel ui production dep |
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
