---
id: T-174
type: task
title: Wire Current Speed into metric card
status: done
priority: high
size: XS
size_source: suggested
size_basis: [T-172]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-055
epic: E-015
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
tags: [frontend, metrics, velocity]
created: 2026-07-27
updated: 2026-07-28T07:27:54.696Z
started_at: 2026-07-27T06:25:20Z
completed_at: 2026-07-27T06:28:48Z
actual_ms: 0
---

# T-174: Wire Current Speed into metric card

## Description

Display the 90-day weekly points average on the Current Speed metric card (e.g. `12.4 pts/wk`), with an empty-state glyph when no history exists.

## Acceptance criteria

- [x] Card shows formatted average weekly points from T-173.
- [x] Empty history shows `—` (or equivalent) without looking like a crash.
- [x] Label/subtitle makes the unit clear (points per week).

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T05:55:45Z | prompt | Marco Mendão | Create epic for project status metrics (total/complete/speed + contributors) styled like neo-brutalism metric cards; include stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:27:20Z | 2026-07-27T06:27:20Z | shared-batch: 0 of 3min by points — implement E-015 (T-174) |
