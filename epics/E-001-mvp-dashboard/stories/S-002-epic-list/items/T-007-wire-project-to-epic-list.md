---
id: T-007
type: task
title: Wire selected project to epic list
status: done
priority: high
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 32
estimate_basis: [calibrated:T-007]
session_cap_minutes: 480
parent: S-002
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
tags: [mvp, epics, integration]
created: 2026-07-21
updated: 2026-07-28T06:16:13.686Z
started_at: 2026-07-21T16:49:52Z
completed_at: 2026-07-21T16:51:19Z
actual_ms: 1920000
---

# T-007: Wire selected project to epic list

## Description

Connect the persisted **master folder** cookie from the setup wizard to discovery, the epic parser, and the list UI: discover projects under the master folder, load epics for each, refetch when the master folder changes, and show errors if discovery or boards become unavailable.

## Acceptance criteria

- [x] Epic list loads from all Taskmark projects discovered under the cookie’s master folder.
- [x] Changing master folder re-runs discovery and reloads epic lists.
- [x] Failure to read the master folder or boards shows an actionable error (including return to wizard).
- [x] End-to-end path works: wizard → discover/validate → list epics per project.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 3 | 2026-07-21T16:51:19Z | prompt | Marco Mendão | Implement S-002 epic list |
| 1 | 2026-07-21T16:24:55Z | prompt | Marco Mendão | Create MVP epic with setup wizard + epic list; create stories and tasks |
| 2 | 2026-07-21T16:31:04Z | feedback | Marco Mendão | Wire master folder discovery to per-project epic lists |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T16:19:19Z | 2026-07-21T16:51:19Z | auto-backfilled: velocity × points (missing work log) |
