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
estimate_minutes: 195
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
updated: 2026-07-24T17:39:50.198Z
started_at: null
completed_at: null
actual_ms: 0
---
# S-051: Publishable npm CLI for local board UI

## User story

As a developer with a Taskmark board on disk, I want to run a single npm/npx command that starts the board UI already pointed at that folder, so I do not need to clone or configure `taskmark-frontend`.

## Acceptance criteria

- [ ] A publishable package (working name `@taskmark/ui`) exposes a `bin` that starts the prebuilt Next server.
- [ ] The CLI resolves the board from cwd/env (S-050) before listen.
- [ ] `npx @taskmark/ui` (or agreed name) opens the UI in the browser against the local board.
- [ ] README documents install, `npx`, and `npm start` / script usage.

## Tasks

- [T-153: Configure Next standalone output for packaging](items/T-153-next-standalone-output.md)
- [T-154: Create publishable package with CLI bin](items/T-154-publishable-package-bin.md)
- [T-155: CLI starts server and opens browser](items/T-155-cli-start-open-browser.md)
- [T-156: Document npx and npm start usage](items/T-156-document-npx-npm-start.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for zero-config npm/CLI board UI (no Docker) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
