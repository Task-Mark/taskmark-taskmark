---
id: T-MM-94c78454
type: task
title: Build weekly completed story-points series
status: done
priority: high
size: S
points: 3
parent: S-MM-2d3bf631
epic: E-015
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
tags: [frontend, metrics, overall]
created: 2026-08-29
updated: 2026-08-29T18:30:00Z
started_at: 2026-08-29T18:05:00Z
completed_at: 2026-08-29T18:09:45Z
---

# T-MM-94c78454: Build weekly completed story-points series

## Description

Produce a heatmap-ready series of ISO weeks with completed story points. Reuse existing leaf completion samples and weekly point sums; fill every week in a sensible display window (about one year ending at the current ISO week, or spanning first-to-last completion when that is shorter) so empty weeks are zeros, not missing cells.

## Acceptance criteria

- [x] Series values are sums of `points` on **done** task/bug leaves grouped by ISO week of `completed_at`; items without a parseable completion date or without positive points do not add to a week
- [x] Shelved, cancelled, and parent (epic/story) rollup points are not counted
- [x] Every week in the chosen window has a cell, including zeros
- [x] Unit tests cover empty boards, a single done leaf, and two leaves in the same week

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:46:00Z | prompt | Marco Mendão | Add an 8StarLabs-style heatmap on Overall for story points completed per week, in the board’s retro style, with strong UI/UX. |
| 2026-08-29T18:05:00Z | prompt | Marco Mendão | /tkmd-do S-MM-225ab050 and S-MM-2d3bf631 |
| 2026-08-29T18:20:00Z | feedback | Marco Mendão | Full-year calendar requested, so the series now groups completed points by day inside each ISO week column. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T18:08:15Z | 2026-08-29T18:08:45Z | Weekly completed story-points series with tests for empty, single, and same-week leaves. |
| Marco Mendão | 2026-08-29T18:20:00Z | 2026-08-29T18:30:00Z | Replaced the weekly series with a one-year daily calendar series and tests. |
