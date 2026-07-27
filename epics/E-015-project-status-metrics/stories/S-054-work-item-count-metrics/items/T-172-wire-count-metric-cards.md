---
id: T-172
type: task
title: Wire count metrics into Total and Complete cards
status: done
priority: high
size: XS
size_source: suggested
size_basis: [T-069, T-064]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-054
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
tags: [frontend, metrics, counts]
created: 2026-07-27
updated: 2026-07-27T07:36:40.469Z
started_at: 2026-07-27T06:25:20Z
completed_at: 2026-07-27T06:28:48Z
actual_ms: 0
---

# T-172: Wire count metrics into Total and Complete cards

## Description

Connect the count aggregator to the Total Workitems and Complete Workitems metric cards so they show live values for the active board.

## Acceptance criteria

- [x] Total and Complete cards display the aggregated numbers.
- [x] Switching project / reloading board refreshes the values.
- [x] Labels read clearly as Total / Complete work items (stories, bugs, tasks).

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
| 1 | Marco Mendão | 2026-07-27T06:26:20Z | 2026-07-27T06:26:20Z | shared-batch: 0 of 3min by points — implement E-015 (T-172) |
