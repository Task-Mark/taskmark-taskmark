---
id: T-141
type: task
title: Primary hover underline under Taskmark brand
status: done
priority: low
size: XS
size_source: suggested
size_basis: [similar:T-009]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 8
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-003
epic: E-001
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
tags: [app-bar, brand, ui]
created: 2026-07-24
updated: 2026-07-28T08:37:10.649Z
started_at: 2026-07-24T17:06:11Z
completed_at: 2026-07-24T17:14:20Z
actual_ms: 489000
---
# T-141: Primary hover underline under Taskmark brand

## Description

Show a primary-colored underline under the Taskmark brand text in the app bar, only on hover. The stroke should feel hand-drawn: thicker overall, thin at the start and wider at the end.

## Acceptance criteria

- [x] App bar Taskmark text shows a primary-color underline on hover.
- [x] Underline is not visible when not hovered.
- [x] Underline is taller/thicker and tapers thin→thick like a hand-drawn mark.
- [x] Logo sits beside the brand text and projects/workspaces subtitle, vertically aligned.

## Notes

UI polish on the app bar brand mark.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:06:11Z | prompt | Marco Mendão | Add primary underline below Taskmark text on hover only |
| 2 | 2026-07-24T17:07:39Z | prompt | Marco Mendão | Underline taller; thin at start, thicker at end like hand-drawn |
| 3 | 2026-07-24T17:09:17Z | prompt | Marco Mendão | Stroke should be linear and constant, not wavy |
| 4 | 2026-07-24T17:09:57Z | prompt | Marco Mendão | Underline a bit bigger than the text |
| 5 | 2026-07-24T17:10:28Z | prompt | Marco Mendão | Extend underline more on the right side |
| 6 | 2026-07-24T17:11:07Z | prompt | Marco Mendão | Tilt the Taskmark text a little on hover |
| 7 | 2026-07-24T17:12:30Z | prompt | Marco Mendão | Shift projects/workspaces line down on hover so tilt does not collide |
| 8 | 2026-07-24T17:13:12Z | prompt | Marco Mendão | Add logo.png aligned with Taskmark text and projects/workspaces line |
| 9 | 2026-07-24T17:15:02Z | prompt | Marco Mendão | Expand logo a little on text hover; keep logo from colliding with text |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 316e73a | taskmark-frontend | 2026-07-24T17:14:23Z | Marco Mendão | add brand logo and hover underline |
| 8c8d50e | taskmark-taskmark | 2026-07-24T17:14:44Z | Marco Mendão | complete t-141 brand hover underline |
| 3aec186 | taskmark-frontend | 2026-07-24T17:16:42Z | Marco Mendão | expand logo on brand hover |
| 3a846df | taskmark-taskmark | 2026-07-24T17:16:42Z | Marco Mendão | log t-141 logo hover scale |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T17:06:11Z | 2026-07-24T17:14:20Z | brand logo, hand-drawn hover underline, tilt and subtitle shift |
