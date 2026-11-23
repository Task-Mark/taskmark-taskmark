---
id: B-015
type: bug
title: "taskmark serve fails: Cannot find module './cpu-profile'"
status: shelved
priority: high
size: M
size_source: suggested
size_basis: [B-012]
points: 3
points_source: suggested
estimate_minutes: 30
actual_minutes: 480
estimate_source: suggested
estimate_basis: [speed:90d:10min/pt]
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
tags: [packaging, next, serve, npm]
created: 2026-08-10
updated: 2026-08-29T11:09:34Z
started_at: 2026-08-10T14:31:05Z
completed_at: 2026-08-29T11:09:34Z
actual_ms: 28800000
---
# B-015: taskmark serve fails: Cannot find module './cpu-profile'

## Description

`taskmark serve` / `yarn start` on a board with `@taskmark/ui` crashes immediately: Next’s `start-server.js` requires `./cpu-profile`, but the published standalone tree under `dist/standalone/node_modules/next` is nearly empty (npm always strips nested `node_modules` on pack).

## Repro steps

1. In a dedicated board folder with `@taskmark/ui` installed: `yarn start` or `npx taskmark serve`.
2. Observe `Error: Cannot find module './cpu-profile'`.

## Fix criteria

- [ ] `npm pack` / published tarball includes the full Next standalone dependency tree (rename nested `node_modules` so npm does not strip it).
- [ ] `taskmark serve` restores that tree as `node_modules` before spawning `server.js`.
- [ ] `yarn start` / `npm start` on a board folder reaches Ready on port 8275.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-10T14:31:05Z | prompt | Marco Mendão | Fix yarn start cpu-profile; add yarn dev with MD reload |
| 2 | 2026-08-29T11:09:34Z | prompt | Marco Mendão | Shelve incomplete work on E-001, E-014, and E-021 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 61a5097 | taskmark-taskmark | 2026-08-10T16:09:57+01:00 | Marco Mendão | sync taskmark board |
| 4db830e | taskmark-frontend | 2026-08-10T15:09:00Z | Marco Mendão | fix serve packaging and add taskmark dev |
| ac89ac0 | taskmark-cursor | 2026-08-10T15:09:00Z | Marco Mendão | point board stub dev at taskmark dev |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-08-10T14:31:05Z | — | In progress: fix serve packaging + add taskmark dev |
