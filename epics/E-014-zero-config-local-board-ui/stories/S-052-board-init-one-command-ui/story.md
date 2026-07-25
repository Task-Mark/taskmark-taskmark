---
id: S-052
type: story
title: Board init one-command UI launch
status: backlog
priority: medium
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 70
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
tags: [plugin, init, cli, docs]
created: 2026-07-24
updated: 2026-07-25T10:44:19.816Z
started_at: null
completed_at: null
actual_ms: 0
---
# S-052: Board init one-command UI launch

## User story

As someone whose Cursor/plugin just created a Taskmark board, I want to be told to run `npx taskmark serve` (port 8275) so the web UI opens against that board without setting up a frontend project.

## Acceptance criteria

- [ ] Board init / README documents `npx taskmark serve` and `http://localhost:8275` from product root or board root.
- [ ] Optional stub `package.json` can expose a script that runs `taskmark serve` (e.g. `"start": "taskmark serve"`).
- [ ] Instructions cover both nested `taskmark/` and flat dedicated board roots.

## Tasks

- [T-157: Document one-command UI launch on board init](items/T-157-document-one-command-on-init.md)
- [T-158: Optional stub package.json for npm start](items/T-158-optional-stub-package-json.md)

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
