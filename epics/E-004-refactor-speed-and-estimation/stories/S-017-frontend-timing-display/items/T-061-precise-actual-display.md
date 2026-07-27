---
id: T-061
type: task
title: Show precise Actual with seconds or milliseconds
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-045, T-046]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 2
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-017
epic: E-004
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
tags: [frontend, actual, timing]
created: 2026-07-22
updated: 2026-07-27T05:16:43.229Z
started_at: 2026-07-22T00:13:39Z
completed_at: 2026-07-22T00:16:21Z
actual_ms: 162000
---

# T-061: Show precise Actual with seconds or milliseconds

## Description

Actual is floored to whole minutes, so short or shared-batch slices show as `0m`. Persist precise billable time and display seconds/milliseconds when useful on task and story (and epic) views.

## Acceptance criteria

- [x] recompute writes `actual_ms` from work-log billable span; `actual_minutes` remains floor(ms/60000) for velocity.
- [x] Shared-batch allocation splits milliseconds by points (sum equals batch ms).
- [x] Lists and detail sheets format Actual with ms/s when under a minute (or leftover seconds), else compact m/h/d.
- [x] Story and task lists show the precise Actual (epics too for consistency).

## Notes

Est stays minute-oriented.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-22T00:13:39Z | prompt | Marco Mendão | Show actual time spent to the milliseconds if need on tasks and user stories |
| 2 | 2026-07-22T00:16:21Z | feedback | Marco Mendão | Precise Actual display delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| ff5d088 | taskmark-frontend | 2026-07-22T00:17:56Z | Marco Mendão | show precise actual duration |
| 0b6df50 | taskmark-taskmark | 2026-07-22T00:17:57Z | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-22T00:13:39Z | 2026-07-22T00:16:21Z | Precise Actual ms display + recompute actual_ms |
