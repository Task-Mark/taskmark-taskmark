---
id: S-051
type: story
title: Publishable npm CLI for local board UI
status: done
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 16
points_source: rolled_up
estimate_minutes: 185
actual_minutes: 6
estimate_source: suggested
estimate_basis: [sum:tasks]
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
tags: [frontend, packaging, cli, npm]
created: 2026-07-24
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-28T08:31:48Z
completed_at: 2026-07-28T09:10:14Z
actual_ms: 383667
---

# S-051: Publishable npm CLI for local board UI

## User story

As a developer with a Taskmark board on disk, I want to run `npx taskmark serve` so the board UI starts on port 8275 already pointed at that folder, without cloning or configuring `taskmark-frontend`.

## Acceptance criteria

- [x] Publishable package exposes bin `taskmark` with subcommand `serve` that starts the prebuilt Next server.
- [x] The CLI resolves the board from cwd/env (S-050) before listen.
- [x] `npx taskmark serve` opens the UI in the browser at `http://localhost:8275` against the local board.
- [x] Default listen port is **8275**; override via flag and/or env is allowed.
- [x] README documents `npx taskmark serve`, port 8275, and optional local script wrappers.

## Tasks

- [T-153: Configure Next standalone output for packaging](items/T-153-next-standalone-output.md)
- [T-154: Create publishable package with CLI bin](items/T-154-publishable-package-bin.md)
- [T-155: CLI starts server and opens browser](items/T-155-cli-start-open-browser.md)
- [T-156: Document npx and npm start usage](items/T-156-document-npx-npm-start.md)
- [T-241: Publish local UI as scoped package @taskmark/ui](items/T-241-publish-scoped-taskmark-ui.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for zero-config npm/CLI board UI (no Docker) |
| 2 | 2026-07-25T10:21:15Z | prompt | Marco Mendão | CLI must be `npx taskmark serve`; default port 8275 |
| 3 | 2026-07-28T08:31:48Z | prompt | Marco Mendão | Implement E-014 remaining stories: publishable npm CLI (taskmark serve, port 8275) and board-init one-command UI launch docs/stub |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 31800fc | taskmark-taskmark | 2026-07-28T09:13:02Z | Marco Mendão | log T-241 @taskmark/ui commits |
| b62a48c | taskmark-frontend | 2026-07-28T09:12:29Z | Marco Mendão | publish local ui as @taskmark/ui |
| bce55d8 | taskmark-cursor | 2026-07-28T09:12:29Z | Marco Mendão | point board init at @taskmark/ui |
| bd0fede | taskmark-taskmark | 2026-07-28T09:12:29Z | Marco Mendão | sync taskmark board |
| f9b7f3f | taskmark-frontend | 2026-07-28T09:50:48Z | Marco Mendão | add taskmark serve cli and zero-config board bind |
| 935c164 | taskmark-taskmark | 2026-07-28T09:50:56Z | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T08:31:48Z | 2026-07-28T08:31:48Z | Rollup: S-051 CLI packaging done (shared-batch on leaves); 0-min parent rollup |
