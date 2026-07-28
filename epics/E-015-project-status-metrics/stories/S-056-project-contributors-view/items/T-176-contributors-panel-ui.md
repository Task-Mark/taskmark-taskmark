---
id: T-176
type: task
title: Build contributors panel UI
status: done
priority: medium
size: M
size_source: suggested
size_basis: [T-121, T-119]
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-056
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
tags: [frontend, contributors, ui]
created: 2026-07-27
updated: 2026-07-28T15:03:07.151Z
started_at: 2026-07-27T06:25:20Z
completed_at: 2026-07-27T06:28:48Z
actual_ms: 60000
---

# T-176: Build contributors panel UI

## Description

Simple contributors panel near the metrics strip: initials avatars (reuse attribution avatar primitives) with name labels. Keep it a lightweight list/grid — not a full people admin page.

## Acceptance criteria

- [x] Renders unique contributors from T-175.
- [x] Shows initials avatar + display name; email on hover/title.
- [x] Empty state copy when the list is empty.
- [x] Visually aligned with metrics strip (same overview region).

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
| 1 | Marco Mendão | 2026-07-27T06:27:20Z | 2026-07-27T06:28:20Z | shared-batch: 1 of 3min by points — implement E-015 (T-176) |
