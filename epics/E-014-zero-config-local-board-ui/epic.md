---
id: E-014
type: epic
title: Zero-config local board UI package
status: backlog
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 27
points_source: rolled_up
estimate_minutes: 380
actual_minutes: 0
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
resolvers: []
blocked: false
cancelled: false
tags: [frontend, packaging, cli, npm, local]
created: 2026-07-24
updated: 2026-07-28T07:27:54.696Z
started_at: null
completed_at: null
actual_ms: 0
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

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
