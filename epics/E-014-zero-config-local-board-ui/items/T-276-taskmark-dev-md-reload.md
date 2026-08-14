---
id: T-276
type: task
title: Add taskmark dev with board markdown live reload
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-154]
points: 3
points_source: suggested
estimate_minutes: 35
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:12min/pt]
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
tags: [cli, frontend, dx, watch]
created: 2026-08-10
updated: 2026-08-14T17:50:46.835Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-276: Add taskmark dev with board markdown live reload

## Description

Board stubs currently map `dev` to `taskmark serve` (production standalone). Add `taskmark dev` that runs Next in development against the resolved board and refreshes the UI when board `.md` files change.

## Acceptance criteria

- [ ] CLI exposes `taskmark dev` (port 8275 by default, same board resolution as serve).
- [ ] Board stub / init `package.json` uses `"dev": "taskmark dev"`.
- [ ] Editing a board markdown file triggers a UI refresh without restarting the process.
- [ ] README documents `taskmark dev` vs `taskmark serve`.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-10T14:31:05Z | prompt | Marco Mendão | Fix yarn start cpu-profile; add yarn dev with MD reload |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 61a5097 | taskmark-taskmark | 2026-08-10T16:09:57+01:00 | Marco Mendão | sync taskmark board |
| 4db830e | taskmark-frontend | 2026-08-10T15:09:00Z | Marco Mendão | fix serve packaging and add taskmark dev |
| ac89ac0 | taskmark-cursor | 2026-08-10T15:09:00Z | Marco Mendão | point board stub dev at taskmark dev |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
