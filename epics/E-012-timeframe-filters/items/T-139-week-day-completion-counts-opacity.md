---
id: T-139
type: task
title: Week/day completion counts and prev/next opacity
status: done
priority: medium
size: M
size_source: suggested
size_basis: [velocity:similar]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 2
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: E-012
epic: E-012
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
tags: [filters, timeframe, weeks, frontend, ui]
created: 2026-07-24
updated: 2026-07-28T09:08:49.505Z
started_at: 2026-07-24T16:46:51Z
completed_at: 2026-07-24T16:49:27Z
actual_ms: 156000
---
# T-139: Week/day completion counts and prev/next opacity

## Description

Prev/next week rows use the same primary tint as each other with higher opacity than the current week. Show completed counts per week and per calendar day for stories + epic-direct tasks/bugs only (exclude tasks under a story).

## Acceptance criteria

- [x] Prev and next week backgrounds match, with higher opacity than the current week.
- [x] Each week in the picker shows a completion count.
- [x] Calendar days show the same completion count.
- [x] Counts include user stories and epic-direct tasks/bugs only (not story subtasks).

## Notes

Follow-up polish on E-012.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T16:46:51Z | prompt | Marco Mendão | More opacity on prev/next vs current; show completed story+epic-direct counts on weeks and calendar |
| 2 | 2026-07-24T16:50:31Z | prompt | Marco Mendão | Swap current vs prev/next week background opacity |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| f85e61c | taskmark-frontend | 2026-07-24T16:54:00Z | Marco Mendão | add timeframe filters for solved work items |
| ea2c152 | taskmark-taskmark | 2026-07-24T16:54:00Z | Marco Mendão | complete e-012 timeframe filters |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T16:46:51Z | 2026-07-24T16:49:27Z | prev/next bg-primary/40 vs current /5; week+calendar completion counts |
