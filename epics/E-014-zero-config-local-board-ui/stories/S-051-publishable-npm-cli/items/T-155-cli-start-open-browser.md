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
estimate_minutes: 45
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
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
updated: 2026-07-24T17:39:50.198Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-155: CLI starts server and opens browser

## Description

Implement the CLI entry: resolve board from cwd/env, set the auto-config env for the server process, listen on a local port, and open the default browser to the board URL.

## Acceptance criteria

- [ ] CLI fails with a clear message when no board can be resolved.
- [ ] Server starts with board auto-config so the UI skips setup.
- [ ] Browser opens to the local board URL (or prints the URL if open is unavailable).
- [ ] Port is configurable (flag or env) with a sensible default.

## Notes

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
