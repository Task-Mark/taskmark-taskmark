---
id: S-004
type: story
title: Add project accumulates workspaces
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 480
actual_minutes: 48
estimate_basis: []
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
tags: [mvp, app-bar, setup]
created: 2026-07-21
updated: 2026-07-28T15:03:07.151Z
started_at: 2026-07-21T17:05:52Z
completed_at: 2026-07-21T17:05:52Z
actual_ms: 2880000
---

# S-004: Add project accumulates workspaces

## User story

As a user, I want **Add project** (not replace master folder) so previously configured projects stay in the dropdown, and duplicate boards discovered under overlapping folders appear only once.

## Acceptance criteria

- [x] App bar uses **Add project** and opens the setup wizard without clearing existing projects.
- [x] Saving a new master folder merges discovered projects into the existing list.
- [x] Projects that resolve to the same `taskmark/` board path are shown once.
- [x] Setup add-mode copy explains that existing projects are kept; cancel returns to board.

## Tasks

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T17:05:52Z | feedback | Marco Mendão | Change master folder should be Add project; keep prior projects; dedupe identical boards |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 5735f0b | taskmark-frontend | 2026-07-21T17:11:35Z | Marco Mendão | add app bar and project accumulate |
| 3389ae7 | taskmark-cursor | 2026-07-21T17:11:35Z | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T16:17:52Z | 2026-07-21T17:05:52Z | auto-backfilled: velocity × points (missing work log) |
