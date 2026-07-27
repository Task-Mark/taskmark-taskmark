---
id: T-162
type: task
title: Persist each Hide completed toggle in a cookie
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-106]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: S-038
epic: E-010
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
tags: [dashboard, frontend, filters]
created: 2026-07-25
updated: 2026-07-27T05:18:44.416Z
started_at: 2026-07-25T21:53:12Z
completed_at: 2026-07-26T12:00:00Z
actual_ms: 0
---

# T-162: Persist each Hide completed toggle in a cookie

## Description

Each list’s **Hide completed** switch should remember its last state across page refresh via a cookie. Epics, overall work items, sub-tasks, work items (and stories if present) each have their own cookie so toggles do not overwrite each other.

## Acceptance criteria

- [x] Refreshing the board keeps each Hide completed switch in its last on/off state.
- [x] Epics, overall work items, sub-tasks, and work-items views each persist independently.
- [x] Default remains off when no cookie is set.
- [x] Server-rendered initial state matches the cookie (no hydration flash).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-25T21:53:12Z | prompt | Marco Mendão | Persist hide toggle in cookie; one persist per toggle |
| 2 | 2026-07-25T21:54:12Z | feedback | Marco Mendão | Implemented per-list cookies + SSR initial state |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| b13c67c | taskmark-frontend | 2026-07-27T06:18:24+01:00 | Marco Mendão | persist hide filters, brand logo, and story progress |
| 3235283 | taskmark-taskmark | 2026-07-27T06:18:25+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Duration | Note |
|---------|-------|---------------|-------------|----------|------|
| 1 | Marco Mendão | 2026-07-25T21:53:12Z | 2026-07-26T12:00:00Z | — | Per-list hide-completed cookies; auto-closed: idle cap (next-day 12:00 UTC) |
