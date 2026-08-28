---
id: T-152
type: task
title: Prefer env and cwd over cookies when auto-config present
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-010, T-004]
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
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-07-28T08:09:03Z
completed_at: 2026-07-28T08:21:03Z
actual_ms: 160000
---

# T-152: Prefer env and cwd over cookies when auto-config present

## Description

Define precedence: env → cwd auto-config → cookie masters. When auto-config is present, board actions and active-project selection use that workspace so stale cookies cannot point at another machine path.

## Acceptance criteria

- [x] Documented precedence is applied in workspace loading.
- [x] Auto-config workspace is what `/board` and detail loaders use when present.
- [x] Cookie-only mode unchanged when auto-config is absent.

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
| 1 | Marco Mendão | 2026-07-28T08:09:03.000Z | 2026-07-28T08:11:43.000Z | Prefer autoconfig over cookies; hide Add project when bound; shared-batch: 160000 of 720000ms by points |
