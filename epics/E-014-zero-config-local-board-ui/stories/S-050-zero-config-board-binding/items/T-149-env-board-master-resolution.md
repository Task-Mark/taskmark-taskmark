---
id: T-149
type: task
title: Add TASKMARK_BOARD and TASKMARK_MASTER env resolution
status: backlog
priority: high
size: S
size_source: suggested
size_basis: [T-003, T-008]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
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
resolvers: []
blocked: false
cancelled: false
tags: [frontend, local, config]
created: 2026-07-24
updated: 2026-07-27T05:30:10.150Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-149: Add TASKMARK_BOARD and TASKMARK_MASTER env resolution

## Description

Introduce shared helpers that read `TASKMARK_BOARD` (exact board path) and `TASKMARK_MASTER` (discovery root), validate them with existing discover/validate logic, and return a configured workspace.

## Acceptance criteria

- [ ] Env vars are resolved to absolute paths and validated.
- [ ] Invalid paths produce a clear error (no silent fallback that looks like empty setup).
- [ ] Helper is usable from server entrypoints (pages/actions) without cookies.

## Notes

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
