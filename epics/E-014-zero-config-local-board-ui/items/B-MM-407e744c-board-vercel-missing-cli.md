---
id: B-MM-407e744c
type: bug
title: Vercel board build cannot find the taskmark CLI
status: done
priority: high
size: S
points: 3
parent: E-014
epic: E-014
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
tags: [vercel, npm, board, packaging]
created: 2026-09-15
updated: 2026-09-15T23:35:56Z
started_at: 2026-09-15T23:26:00Z
completed_at: 2026-09-15T23:35:56Z
---
# B-MM-407e744c: Vercel board build cannot find the taskmark CLI

## Description

The hosted board Vercel build runs `npm install` then `taskmark build --board . --out out` and exits 127 (`taskmark: command not found`). The board depends on `@taskmark/ui` via `file:../taskmark-frontend`, which Vercel does not clone, so the CLI never lands on `PATH`. Vercel also warns that `engines.node` of `>=18` will auto-upgrade on a new major.

## User story

As a visitor, I want the public board site to build on Vercel so the live Taskmark board stays available after a release.

## Fix criteria

- [x] The board depends on the published `@taskmark/ui` SemVer, not a sibling `file:` path.
- [x] `npm install` on a standalone board clone puts the `taskmark` bin on `PATH`.
- [x] Board `engines.node` is a Vercel-safe major pin, not an open `>=` range.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:26:00Z | prompt | Marco Mendão | Vercel board build cannot find `taskmark`, and Vercel warns about `engines.node` `>=18`. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T23:26:00Z | 2026-09-15T23:35:56Z | Pointed the board at published `@taskmark/ui@1.2.0`, pinned `engines.node` to `22.x`, and removed the sibling `file:` lockfile. |
