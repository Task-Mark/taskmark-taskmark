---
id: S-001
type: story
title: Project setup wizard
status: done
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 13
points_source: rolled_up
estimate_minutes: 115
actual_minutes: 206
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-001
epic: E-001
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
tags: [mvp, wizard, setup]
created: 2026-07-21
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-21T16:35:18Z
completed_at: 2026-07-21T16:37:18Z
actual_ms: 12360000
---

# S-001: Project setup wizard

## User story

As a user, I want a setup wizard that lets me select a local **master folder** so the dashboard can discover one or more Taskmark projects in its subfolders.

## Acceptance criteria

- [x] First-run (or no master-folder cookie) shows a setup wizard, not an empty dashboard.
- [x] User can choose a local **master folder** path (workspace that may contain multiple projects).
- [x] App discovers Taskmark boards by scanning **subfolders** (does not require `taskmark/` only at the master root).
- [x] App validates that at least one Taskmark project is found (or shows a clear error if none).
- [x] Valid master folder is persisted in a **cookie** and the user continues into the app (epic lists).
- [x] Returning users with a master-folder cookie skip setup entirely — they are not required to set up again.
- [x] User can reopen setup to **switch** master folders; the new selection replaces the cookie.

## Tasks

- [T-001: Build setup wizard UI shell](items/T-001-setup-wizard-ui.md)
- [T-002: Implement project folder selection](items/T-002-folder-selection.md)
- [T-003: Validate taskmark board in selected folder](items/T-003-validate-taskmark-board.md)
- [T-004: Persist selected project and enter app](items/T-004-persist-project-selection.md)
- [T-008: Discover Taskmark projects under master folder](items/T-008-discover-projects-under-master.md)
- [B-003: Setup fails to discover flat multi-repo board](items/B-003-discover-flat-taskmark-board.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T16:24:55Z | prompt | Marco Mendão | Create MVP epic with setup wizard + epic list; create stories and tasks |
| 2 | 2026-07-21T16:29:20Z | feedback | Marco Mendão | Persist project in cookies; skip setup when already configured; allow switching projects via setup |
| 3 | 2026-07-21T16:31:04Z | feedback | Marco Mendão | Master folder may contain multiple Taskmark projects in subfolders; discover by venturing into children |
| 4 | 2026-07-21T16:35:18Z | prompt | Marco Mendão | Start implementing S-001 project setup wizard |

| 5 | 2026-07-21T22:44:32Z | prompt | Marco Mendão | Setup fails: flat *-taskmark board not discovered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 1fcb25f | taskmark-frontend | 2026-07-21T16:48:57Z | Marco Mendão | add native folder picker to setup |
| e1923e9 | taskmark-cursor | 2026-07-21T16:48:57Z | Marco Mendão | sync taskmark board |
| 9c3c5c5 | taskmark-frontend | 2026-07-21T16:40:53Z | Marco Mendão | add setup wizard and taskmark board |
| 489cdff | taskmark-cursor | 2026-07-21T16:40:54Z | Marco Mendão | add taskmark board and update plugin |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T13:11:18Z | 2026-07-21T16:37:18Z | auto-backfilled: rollup from children (missing/under-logged) |
