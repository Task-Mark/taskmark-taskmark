---
id: S-050
type: story
title: Zero-config board binding from env and cwd
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 9
points_source: rolled_up
estimate_minutes: 95
actual_minutes: 12
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-014
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
tags: [frontend, local, config]
created: 2026-07-24
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-28T08:09:03Z
completed_at: 2026-07-28T08:21:03Z
actual_ms: 720000
---

# S-050: Zero-config board binding from env and cwd

## User story

As a developer running the Taskmark UI against a known local board, I want the app to bind automatically from environment variables or the current working directory, so I never have to use the setup wizard for the common case.

## Acceptance criteria

- [x] `TASKMARK_BOARD` and/or `TASKMARK_MASTER` resolve a valid workspace without cookies.
- [x] When cwd is a board root or a product root containing `./taskmark/`, discovery binds that board.
- [x] With valid auto-config, `/` and `/board` never redirect to `/setup`.
- [x] Existing cookie-based multi-master setup remains available when auto-config is absent.

## Tasks

- [T-149: Add TASKMARK_BOARD and TASKMARK_MASTER env resolution](items/T-149-env-board-master-resolution.md)
- [T-150: Resolve board from cwd layouts](items/T-150-resolve-board-from-cwd.md)
- [T-151: Skip setup wizard when auto-config is valid](items/T-151-skip-setup-when-autoconfig.md)
- [T-152: Prefer env and cwd over cookies when auto-config present](items/T-152-prefer-autoconfig-over-cookies.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for zero-config npm/CLI board UI (no Docker) |
| 2 | 2026-07-28T08:09:03Z | prompt | Marco Mendão | Implement zero-config: npm run dev in taskmark-frontend keeps setup; when a local taskmark folder exists for the project, show only that project's board |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| f9b7f3f | taskmark-frontend | 2026-07-28T09:50:48Z | Marco Mendão | add taskmark serve cli and zero-config board bind |
| 935c164 | taskmark-taskmark | 2026-07-28T09:50:56Z | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T08:09:03Z | 2026-07-28T08:09:03Z | shared-batch rollup: children hold billable minutes |
