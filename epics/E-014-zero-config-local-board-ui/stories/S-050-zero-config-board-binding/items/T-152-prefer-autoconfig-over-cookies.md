---
id: T-152
type: task
title: Prefer env and cwd over cookies when auto-config present
status: backlog
priority: medium
size: S
size_source: suggested
size_basis: [T-010, T-004]
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
updated: 2026-07-27T07:45:28.202Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-152: Prefer env and cwd over cookies when auto-config present

## Description

Define precedence: env → cwd auto-config → cookie masters. When auto-config is present, board actions and active-project selection use that workspace so stale cookies cannot point at another machine path.

## Acceptance criteria

- [ ] Documented precedence is applied in workspace loading.
- [ ] Auto-config workspace is what `/board` and detail loaders use when present.
- [ ] Cookie-only mode unchanged when auto-config is absent.

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
