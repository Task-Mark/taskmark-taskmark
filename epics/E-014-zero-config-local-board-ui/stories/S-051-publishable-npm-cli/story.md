---
id: S-051
type: story
title: Publishable npm CLI for local board UI
status: backlog
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 13
points_source: rolled_up
estimate_minutes: 180
actual_minutes: 0
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
resolvers: []
blocked: false
cancelled: false
tags: [frontend, packaging, cli, npm]
created: 2026-07-24
updated: 2026-07-25T10:24:50.747Z
started_at: null
completed_at: null
actual_ms: 0
---

# S-051: Publishable npm CLI for local board UI

## User story

As a developer with a Taskmark board on disk, I want to run `npx taskmark serve` so the board UI starts on port 8275 already pointed at that folder, without cloning or configuring `taskmark-frontend`.

## Acceptance criteria

- [ ] Publishable package exposes bin `taskmark` with subcommand `serve` that starts the prebuilt Next server.
- [ ] The CLI resolves the board from cwd/env (S-050) before listen.
- [ ] `npx taskmark serve` opens the UI in the browser at `http://localhost:8275` against the local board.
- [ ] Default listen port is **8275**; override via flag and/or env is allowed.
- [ ] README documents `npx taskmark serve`, port 8275, and optional local script wrappers.

## Tasks

- [T-153: Configure Next standalone output for packaging](items/T-153-next-standalone-output.md)
- [T-154: Create publishable package with CLI bin](items/T-154-publishable-package-bin.md)
- [T-155: CLI starts server and opens browser](items/T-155-cli-start-open-browser.md)
- [T-156: Document npx and npm start usage](items/T-156-document-npx-npm-start.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for zero-config npm/CLI board UI (no Docker) |
| 2 | 2026-07-25T10:21:15Z | prompt | Marco Mendão | CLI must be `npx taskmark serve`; default port 8275 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
