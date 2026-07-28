---
id: T-155
type: task
title: CLI starts server and opens browser
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-154, T-149]
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-051
epic: E-014
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, packaging, cli]
created: 2026-07-24
updated: 2026-07-28T07:41:00.094Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-155: CLI starts server and opens browser

## Description

Implement `taskmark serve`: resolve board from cwd/env, set the auto-config env for the server process, listen on **port 8275** by default, and open the default browser to the board URL.

## Acceptance criteria

- [ ] `taskmark serve` (and thus `npx taskmark serve`) starts the UI server.
- [ ] Default listen port is **8275** (`http://localhost:8275`).
- [ ] Port override via flag (e.g. `--port`) and/or env is supported.
- [ ] CLI fails with a clear message when no board can be resolved.
- [ ] Server starts with board auto-config so the UI skips setup.
- [ ] Browser opens to the local board URL (or prints the URL if open is unavailable).

## Notes

Port **8275** is the product default — do not use Next’s 3000 unless overridden.

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
