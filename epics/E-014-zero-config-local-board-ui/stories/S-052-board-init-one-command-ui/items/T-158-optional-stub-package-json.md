---
id: T-158
type: task
title: Optional stub package.json for npm start
status: done
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
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [plugin, init, npm]
created: 2026-07-24
updated: 2026-07-28T08:37:10.649Z
started_at: 2026-07-28T08:31:48Z
completed_at: 2026-07-28T08:36:30Z
actual_ms: 31333
---
# T-158: Optional stub package.json for npm start

## Description

Optionally scaffold a minimal `package.json` that depends on the `taskmark` package and exposes scripts such as `"start": "taskmark serve"` so users can `npm i && npm start` (still on port **8275**).

## Acceptance criteria

- [x] Stub script runs `taskmark serve` (not a generic Next `dev` on 3000).
- [x] Dependency points at the publishable package that provides bin `taskmark`.
- [x] Scaffolding is opt-in or clearly documented so boards stay markdown-first by default.

## Notes

Prefer documenting `npx taskmark serve` as the default; stub is for users who want a local script.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for zero-config npm/CLI board UI (no Docker) |
| 2 | 2026-07-25T10:21:15Z | prompt | Marco Mendão | CLI must be `npx taskmark serve`; default port 8275 |
| 3 | 2026-07-28T08:31:48Z | prompt | Marco Mendão | Implement E-014 remaining stories: publishable npm CLI (taskmark serve, port 8275) and board-init one-command UI launch docs/stub |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T08:31:48Z | 2026-07-28T08:32:19.333Z | Optional board-ui-stub package.json for npm start; shared-batch: 31333 of 282000ms by points |
