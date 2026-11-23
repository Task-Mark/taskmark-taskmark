---
id: R-zero-config-local-board-ui-package
type: request
title: Zero-config local board UI package
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-24
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - frontend
  - packaging
  - cli
  - npm
  - local
  - vercel
aliases:
  - E-014
source_meetings: []
links: []
---

# Zero-config local board UI package

## Goal

Ship Taskmark’s web UI so a developer can open a local board with `npx taskmark serve` (default port **8275**) — no cloning `taskmark-frontend`, no setup wizard, and no manual path configuration when the board is already on disk.

## Scope

- Auto-bind the UI to a board from env (`TASKMARK_BOARD` / `TASKMARK_MASTER`) or cwd (nested `taskmark/` or flat `*-taskmark` root).
- Skip `/setup` when auto-config is valid; open straight on `/board`.
- Publish an npm package with bin `taskmark` and subcommand `serve` that starts a prebuilt server against the resolved board on port **8275** by default.
- Document (and optionally scaffold) a one-command launch path when a board is created/initialized.

## Done when

- From a product repo with `./taskmark/` (or a dedicated board root), `npx taskmark serve` opens the dashboard at `http://localhost:8275` on that board with no setup steps.
- Cookie-based multi-master setup still works when no auto-config is present.

## Out of scope

- Docker / custom nginx images (Vercel static hosting is in scope via T-258–T-259).
- Hosted/cloud board sync or multi-tenant SaaS.
- Changing board markdown schema beyond what the current UI already reads.

## Open questions

_None yet._
