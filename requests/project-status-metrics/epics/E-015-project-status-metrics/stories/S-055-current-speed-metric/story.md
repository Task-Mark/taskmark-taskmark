---
id: S-055
type: story
title: Current speed metric
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 7
points_source: rolled_up
estimate_minutes: 85
actual_minutes: 1
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-015
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
tags: [frontend, metrics, velocity, speed]
created: 2026-07-27
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-07-27T06:25:20Z
completed_at: 2026-07-27T07:19:27Z
actual_ms: 78000
---

# S-055: Current speed metric

## User story

As a project lead, I want a Current Speed number based on recent weekly throughput, so I can judge delivery pace without opening velocity docs.

## Acceptance criteria

- [x] Find the week containing the most recently completed **task or bug** (`completed_at`); that week anchors the end of the 90-day window.
- [x] Look back **90 days** from that anchor (inclusive of weeks overlapping the window).
- [x] For each week in the window, sum **story points** of tasks/bugs completed that week.
- [x] **Exclude** the **current** ISO week from the average (in-progress week).
- [x] **Exclude** weeks with **0** points (idle/hold) from both numerator and denominator.
- [x] **Current Speed** = sum(remaining weekly totals) / count(remaining weeks).
- [x] If no considered weeks remain, show `—`.
- [x] Value renders in the Current Speed metric card.

## Tasks

- [T-173: Implement 90-day weekly points average](items/T-173-ninety-day-weekly-speed.md)
- [T-174: Wire Current Speed into metric card](items/T-174-wire-current-speed-card.md)
- [T-183: Add current week story points card](items/T-183-current-week-story-points-card.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 2 | 2026-07-27T06:25:20Z | prompt | Marco Mendão | Implement the E-015 |
| 1 | 2026-07-27T05:55:45Z | prompt | Marco Mendão | Create epic for project status metrics (total/complete/speed + contributors) styled like neo-brutalism metric cards; include stories and tasks |
| 3 | 2026-07-27T06:42:30Z | prompt | Marco Mendão | Fix speed: ignore current week and zero-point weeks in average |


## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 577a91d | taskmark-frontend | 2026-07-27T07:16:12Z | Marco Mendão | add current week points metric |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:25:20Z | 2026-07-27T06:25:20Z | Parent rollup: children hold shared-batch |
