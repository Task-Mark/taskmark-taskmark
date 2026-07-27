---
id: T-151
type: task
title: Skip setup wizard when auto-config is valid
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-004, T-010]
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
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
updated: 2026-07-27T07:06:27.645Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-151: Skip setup wizard when auto-config is valid

## Description

Update `/`, `/setup`, and `/board` entry routing so a valid auto-configured workspace goes straight to the board UI instead of the setup wizard.

## Acceptance criteria

- [ ] Valid auto-config → `/` redirects to `/board` (not `/setup`).
- [ ] `/board` loads using the auto-configured project list.
- [ ] Without auto-config and without cookies, existing `/setup` flow still works.

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
