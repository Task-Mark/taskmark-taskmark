---
id: S-MM-07de76ad
type: story
title: Team insight widgets — leaderboard, velocity comparison, task-vs-bug split
status: backlog
priority: medium
size: null
points: null
parent: E-MM-1cc60def
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, dashboard, insights, charts]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# S-MM-07de76ad: Team insight widgets — leaderboard, velocity comparison, task-vs-bug split

## Description

Comparative insight widgets on the dashboard: a contributor leaderboard for the filtered period (points completed and worklog sessions), a per-project velocity comparison (average vs peak pts/week already present in `statusMetrics`), and a task-vs-bug completion split rendered with the shared chart components.

## User story

As a Cloud user, I want rankings and comparisons across people and projects so I can recognise contributions and spot imbalances between feature work and bug fixing.

## Acceptance criteria

- [ ] A leaderboard ranks contributors in the filtered period by points completed, with session counts alongside.
- [ ] A velocity chart compares average and peak pts/week per project, labelling the peak week.
- [ ] A task-vs-bug widget shows the completion split for the filtered period.
