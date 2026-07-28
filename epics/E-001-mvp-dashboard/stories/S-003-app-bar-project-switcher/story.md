---
id: S-003
type: story
title: App bar project switcher
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 12
points_source: rolled_up
estimate_minutes: 540
actual_minutes: 513
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
tags: [mvp, app-bar, navigation]
created: 2026-07-21
updated: 2026-07-28T07:41:00.094Z
started_at: 2026-07-21T16:59:31Z
completed_at: 2026-07-27T05:16:43Z
actual_ms: 30797000
---

# S-003: App bar project switcher

## User story

As a user, after I set up a master folder, I want an app bar that lets me switch among the discovered (pre-configured) Taskmark projects so I can focus on one project’s epics without re-running setup.

## Acceptance criteria

- [x] Post-setup screens show an app bar with the Taskmark brand.
- [x] App bar lists discovered projects from the current master folder.
- [x] User can switch the active project from the app bar without clearing the master folder.
- [x] Active project is persisted (cookie) and restored on return visits.
- [x] Epic list shows the active project (not all projects at once).
- [x] User can still change the master folder from the app bar (setup).

## Tasks

- [B-008: Brand logo sits flush against app bar bottom border](items/B-008-brand-logo-flush-header-border.md)

- [T-009: Build post-setup app bar UI](items/T-009-app-bar-ui.md)
- [T-010: Persist active project and filter epic list](items/T-010-active-project-cookie.md)
- [T-141: Primary hover underline under Taskmark brand](items/T-141-brand-hover-underline.md)
- [T-163: Replace app brand logo with tm_light mark](items/T-163-replace-brand-logo.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T16:59:31Z | prompt | Marco Mendão | After setup, app bar should switch among pre-configured projects |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 5735f0b | taskmark-frontend | 2026-07-21T17:11:35Z | Marco Mendão | add app bar and project accumulate |
| 3389ae7 | taskmark-cursor | 2026-07-21T17:11:35Z | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T16:59:31Z | 2026-07-21T16:59:31Z | App bar project switcher shipped; shared-batch: 0min rollup (children hold allocation) |
| 2 | Marco Mendão | 2026-07-21T16:59:31Z | 2026-07-21T17:11:35Z | auto-recovered: commit span; shared-batch: 0min rollup (children hold allocation) |
