---
id: S-053
type: story
title: Metrics cards UI shell
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 70
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
tags: [frontend, metrics, ui]
created: 2026-07-27
updated: 2026-07-29T11:30:07.936Z
started_at: 2026-07-27T06:25:20Z
completed_at: 2026-07-27T06:28:48Z
actual_ms: 60000
---

# S-053: Metrics cards UI shell

## User story

As a project lead viewing the board, I want a row of metric cards that match the neo-brutalism reference style, so project status is scannable at a glance before I dig into lists.

## Acceptance criteria

- [x] A reusable `MetricStatCard` (or equivalent) renders title, large value, and accent icon with hard black border/shadow.
- [x] A metrics strip on the board can host at least three cards (Total, Complete, Current Speed) in one horizontal composition on desktop and stacks cleanly on small screens.
- [x] Empty / loading placeholders do not break layout when values are not yet available.
- [x] Visual style follows the reference: white surface, solid black borders, bold typography, vibrant icon square — without copying unrelated business KPIs.

## Tasks

- [T-169: Build MetricStatCard component](items/T-169-metric-stat-card-component.md)
- [T-170: Place metrics strip on board overview](items/T-170-metrics-strip-on-board.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 2 | 2026-07-27T06:25:20Z | prompt | Marco Mendão | Implement the E-015 |
| 1 | 2026-07-27T05:55:45Z | prompt | Marco Mendão | Create epic for project status metrics (total/complete/speed + contributors) styled like neo-brutalism metric cards; include stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:25:20Z | 2026-07-27T06:25:20Z | Parent rollup: children hold shared-batch |
