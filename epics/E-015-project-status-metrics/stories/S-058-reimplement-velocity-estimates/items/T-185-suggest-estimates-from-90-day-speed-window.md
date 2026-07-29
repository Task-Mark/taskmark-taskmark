---
id: T-185
type: task
title: Suggest estimates from 90-day speed window
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 1
estimate_source: suggested
estimate_basis: [speed:90d:14min/pt]
session_cap_minutes: 480
parent: S-058
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
tags: [plugin, velocity, estimation]
created: 2026-07-27
updated: 2026-07-29T06:48:27.505Z
started_at: 2026-07-27T07:19:27Z
completed_at: 2026-07-27T07:21:27Z
actual_ms: 60000
---

# T-185: Suggest estimates from 90-day speed window

## Description

Restore estimate suggestion/calibration using median min/pt over the same 90-day done-leaf window; wire create skills.

## Acceptance criteria

- [x] Delivered as described for S-058 redesign.

## Notes

Shared-batch with sibling T-184–T-187 under S-058.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T07:19:27Z | prompt | Marco Mendão | Implement remaining incomplete E-015 work items (S-058) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 21253c0 | taskmark-cursor | 2026-07-27T07:30:51Z | Marco Mendão | restore velocity with current speed |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T07:20:27Z | 2026-07-27T07:21:27Z | Restored 90d median min/pt estimate suggestion + calibrate; shared-batch: 1 of 3min by points |
