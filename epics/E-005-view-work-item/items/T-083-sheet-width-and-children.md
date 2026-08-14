---
id: T-083
type: task
title: Wider detail sheet with epic and story children
status: done
priority: medium
size: M
size_source: suggested
size_basis: [T-055, T-057]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 3
estimate_source: suggested
estimate_basis: [calibrated:T-083]
session_cap_minutes: 480
parent: E-005
epic: E-005
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
tags: [dashboard, frontend, sheet, detail]
created: 2026-07-23
updated: 2026-08-14T17:50:46.835Z
started_at: 2026-07-23T07:09:24Z
completed_at: 2026-07-23T07:12:24Z
actual_ms: 180000
---

# T-083: Wider detail sheet with epic and story children

## Description

Widen the work item detail sheet and show live child lists: stories (and epic-direct tasks) under an epic, tasks/bugs under a story.

## Acceptance criteria

- [x] Sheet is wider than the previous `max-w-xl` width.
- [x] Epic detail shows child stories and epic-direct tasks/bugs (not only markdown links).
- [x] Story detail shows child tasks/bugs.
- [x] Children can open in the same sheet.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T07:09:24Z | prompt | Marco Mendão | Bigger sheet width; show sub stories/tasks on epic and story details |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 6c6195d | taskmark-frontend | 2026-07-23T07:15:40Z | Marco Mendão | widen sheet show children |
| 9c75469 | taskmark-frontend | 2026-07-23T07:15:48Z | Marco Mendão | fix detail sheet layout width |
| 7fa74bf | taskmark-frontend | 2026-07-23T07:16:16Z | Marco Mendão | fix detail sheet table widths |
| 32e276b | taskmark-taskmark | 2026-07-23T07:15:40Z | Marco Mendão | add t-083 sheet children board |
| 34439f4 | taskmark-taskmark | 2026-07-23T07:16:29Z | Marco Mendão | log t-083 commits |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T07:09:24Z | 2026-07-23T07:12:24Z | Wider sheet; epic/story children lists |
