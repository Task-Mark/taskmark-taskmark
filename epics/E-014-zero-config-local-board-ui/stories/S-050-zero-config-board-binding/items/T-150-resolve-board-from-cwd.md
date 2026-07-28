---
id: T-150
type: task
title: Resolve board from cwd layouts
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-008, B-003]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 2
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-050
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
updated: 2026-07-28T09:08:49.505Z
started_at: 2026-07-28T08:09:03Z
completed_at: 2026-07-28T08:21:03Z
actual_ms: 160000
---
# T-150: Resolve board from cwd layouts

## Description

When env vars are unset, resolve a board from `process.cwd()`: treat cwd as a flat dedicated board root, or as a product root with nested `taskmark/`, using the same discovery rules as the setup wizard.

## Acceptance criteria

- [x] Nested `<project>/taskmark/` with INDEX/epics is detected from product cwd.
- [x] Flat `*-taskmark` board root (INDEX/epics at root) is detected when cwd is that root.
- [x] Non-board cwd does not invent a false positive board.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for zero-config npm/CLI board UI (no Docker) |
| 2 | 2026-07-28T08:09:03Z | prompt | Marco Mendão | Implement zero-config: npm run dev in taskmark-frontend keeps setup; when a local taskmark folder exists for the project, show only that project's board |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T08:09:03.000Z | 2026-07-28T08:11:43.000Z | cwd / INIT_CWD / TASKMARK_CWD board resolution; shared-batch: 160000 of 720000ms by points |
