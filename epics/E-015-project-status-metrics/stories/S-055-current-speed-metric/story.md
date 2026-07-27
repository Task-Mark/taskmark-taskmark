---
id: S-055
type: story
title: Current speed metric
status: backlog
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 6
points_source: rolled_up
estimate_minutes: 85
actual_minutes: 0
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
resolvers: []
blocked: false
cancelled: false
tags: [frontend, metrics, velocity, speed]
created: 2026-07-27
updated: 2026-07-27T06:17:22.249Z
started_at: null
completed_at: null
actual_ms: 0
---
# S-055: Current speed metric

## User story

As a project lead, I want a Current Speed number based on recent weekly throughput, so I can judge delivery pace without opening velocity docs.

## Acceptance criteria

- [ ] Find the week containing the most recently completed **task or bug** (`completed_at`); that week is the end of the window.
- [ ] Look back **90 days** from that anchor (inclusive of weeks overlapping the window).
- [ ] For each week in the window, sum **story points** of items completed that week (tasks/bugs that carry points; clarify stories if rolled — prefer leaf done items with points).
- [ ] **Current Speed** = average of those weekly point totals (handle empty weeks as 0 in the average, or document if empty weeks are omitted — pick one and keep consistent).
- [ ] If no completed tasks/bugs exist, show a clear empty state (e.g. `—` or `0`) rather than crashing.
- [ ] Value renders in the Current Speed metric card.

## Tasks

- [T-173: Implement 90-day weekly points average](items/T-173-ninety-day-weekly-speed.md)
- [T-174: Wire Current Speed into metric card](items/T-174-wire-current-speed-card.md)

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
