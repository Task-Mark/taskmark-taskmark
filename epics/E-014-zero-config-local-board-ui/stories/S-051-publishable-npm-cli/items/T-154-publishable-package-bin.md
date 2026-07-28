---
id: T-154
type: task
title: Create publishable package with CLI bin
status: backlog
priority: high
size: L
size_source: suggested
size_basis: [T-153]
points: 5
points_source: suggested
estimate_minutes: 70
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
tags: [frontend, packaging, cli, npm]
created: 2026-07-24
updated: 2026-07-28T07:41:00.094Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-154: Create publishable package with CLI bin

## Description

Create the publishable package so `npx taskmark …` works: `bin.taskmark` points at a Node CLI that supports subcommand `serve`, packages the prebuilt server artifact, and can be installed via npm/`npx`.

## Acceptance criteria

- [ ] Package `bin` is named **`taskmark`** (so `npx taskmark serve` works).
- [ ] CLI parses subcommand `serve` (other subcommands may be stubs/future).
- [ ] Published/packed contents include the prebuilt server needed to run without a source checkout.
- [ ] Package `name` in package.json is chosen so `npx taskmark` resolves the bin (record final name in docs; placeholder OK until publish).

## Notes

Prefer package name `taskmark` on npm if available; otherwise a scoped name that still exposes bin `taskmark`.

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
