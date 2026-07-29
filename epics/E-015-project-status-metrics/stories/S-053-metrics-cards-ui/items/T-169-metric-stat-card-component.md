---
id: T-169
type: task
title: Build MetricStatCard component
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-119, T-068]
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-053
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
updated: 2026-07-29T07:31:14.976Z
started_at: 2026-07-27T06:25:20Z
completed_at: 2026-07-27T06:28:48Z
actual_ms: 60000
---

# T-169: Build MetricStatCard component

## Description

Create a reusable metric card: title (top-left), large bold value, and a colored icon square (top-right) with solid black border and hard offset shadow — matching the neo-brutalism reference image.

## Acceptance criteria

- [x] Props cover title, value (string/number/node), icon, and accent color.
- [x] Card uses white background, solid black border, and readable hierarchy (value much larger than title).
- [x] Icon square has thick black outline + hard black drop-shadow (no soft blur).
- [x] Component is usable from the board metrics strip without list-table dependencies.

## Notes

Trend “vs last period” badge is out of scope for this epic unless trivially stubbed as optional.

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
| 1 | Marco Mendão | 2026-07-27T06:25:20Z | 2026-07-27T06:26:20Z | shared-batch: 1 of 3min by points — implement E-015 (T-169) |
