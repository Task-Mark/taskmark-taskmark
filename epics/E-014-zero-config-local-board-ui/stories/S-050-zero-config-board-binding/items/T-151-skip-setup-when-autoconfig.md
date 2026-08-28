---
id: T-151
type: task
title: Skip setup wizard when auto-config is valid
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-004, T-010]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 4
estimate_source: suggested
estimate_basis: [calibrated:T-151]
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
actual_ms: 240000
---

# T-151: Skip setup wizard when auto-config is valid

## Description

Update `/`, `/setup`, and `/board` entry routing so a valid auto-configured workspace goes straight to the board UI instead of the setup wizard.

## Acceptance criteria

- [x] Valid auto-config → `/` redirects to `/board` (not `/setup`).
- [x] `/board` loads using the auto-configured project list.
- [x] Without auto-config and without cookies, existing `/setup` flow still works.

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
| 1 | Marco Mendão | 2026-07-28T08:09:03.000Z | 2026-07-28T08:13:03.000Z | Skip setup when autoconfig; / goes to /board; shared-batch: 240000 of 720000ms by points |
