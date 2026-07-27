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
updated: 2026-07-27T07:23:21.914Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-158: Optional stub package.json for npm start

## Description

Optionally scaffold a minimal `package.json` that depends on the `taskmark` package and exposes scripts such as `"start": "taskmark serve"` so users can `npm i && npm start` (still on port **8275**).

## Acceptance criteria

- [ ] Stub script runs `taskmark serve` (not a generic Next `dev` on 3000).
- [ ] Dependency points at the publishable package that provides bin `taskmark`.
- [ ] Scaffolding is opt-in or clearly documented so boards stay markdown-first by default.

## Notes

Prefer documenting `npx taskmark serve` as the default; stub is for users who want a local script.

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
