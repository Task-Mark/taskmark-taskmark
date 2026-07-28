---
id: T-180
type: task
title: Show story points per day on calendar picker
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-139]
points: 2
points_source: suggested
estimate_minutes: 0
actual_minutes: 2
estimate_source: suggested
estimate_basis: []
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
tags: [filters, timeframe, calendar, frontend]
created: 2026-07-27
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-27T06:51:07Z
completed_at: 2026-07-27T06:53:47Z
actual_ms: 160000
---

# T-180: Show story points per day on calendar picker

## Description

On the date-range calendar picker, show the sum of story points completed that day (same countable set as existing badges: stories + epic-direct tasks/bugs), not item counts.

## Acceptance criteria

- [x] Calendar day cells show story points completed that day when > 0.
- [x] Data uses completed items with points from the board countable set.
- [x] Empty days remain visually quiet (no misleading zero badge).

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T06:51:07Z | prompt | Marco Mendão | Calendar filter should show story points per day on the picker |
| 2 | 2026-07-27T06:53:47Z | feedback | Marco Mendão | Delivered calendar story-point badges |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| d5f8f02 | taskmark-frontend | 2026-07-27T07:08:31Z | Marco Mendão | add project metrics and calendar points |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:51:07Z | 2026-07-27T06:53:47Z | Calendar day/week badges show story-point sums from countable completions |
