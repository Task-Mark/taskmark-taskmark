---
id: T-183
type: task
title: Add current week story points card
status: done
priority: high
size: XS
size_source: suggested
size_basis: [T-174]
points: 1
points_source: suggested
estimate_minutes: 0
actual_minutes: 0
estimate_source: suggested
estimate_basis: []
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
tags: [frontend, metrics, speed, points]
created: 2026-07-27
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-27T07:09:00Z
completed_at: 2026-07-27T07:09:18Z
actual_ms: 18000
---

# T-183: Add current week story points card

## Description

Add a metric card that shows the total story points completed in the current ISO week, using the same completed task/bug leaf point set as Current Speed.

## Acceptance criteria

- [x] Metric card shows current ISO week completed points.
- [x] Uses the same completed task/bug leaf points as Current Speed.
- [x] Empty state is clear when the current week has no completed points.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T07:09:00Z | prompt | Marco Mendão | Add a metric with the current week storypoints made |
| 2 | 2026-07-27T07:09:18Z | feedback | Marco Mendão | Added current week story points metric card |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 577a91d | taskmark-frontend | 2026-07-27T07:16:12Z | Marco Mendão | add current week points metric |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T07:09:00Z | 2026-07-27T07:09:18Z | Added current week metric card using completed task/bug leaf points |
