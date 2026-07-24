---
id: T-158
type: task
title: Optional stub package.json for npm start
status: backlog
priority: low
size: S
size_source: suggested
size_basis: [T-157]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-052
epic: E-014
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, init, npm]
created: 2026-07-24
updated: 2026-07-24T17:39:50.198Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-158: Optional stub package.json for npm start

## Description

Optionally scaffold a minimal `package.json` (on the board or documented template) that depends on the UI package and exposes `start` / `dev` scripts so users can `npm i && npm start` without memorizing `npx` flags.

## Acceptance criteria

- [ ] Stub (or generator flag) produces a package.json with a script that runs the UI CLI.
- [ ] Dependency points at the publishable package name from S-051.
- [ ] Scaffolding is opt-in or clearly documented so boards stay markdown-first by default.

## Notes

Prefer documenting `npx` as the default; stub is for users who want a local script.

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
