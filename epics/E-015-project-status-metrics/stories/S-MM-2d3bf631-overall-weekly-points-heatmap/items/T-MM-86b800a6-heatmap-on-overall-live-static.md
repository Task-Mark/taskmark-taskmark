---
id: T-MM-86b800a6
type: task
title: Show weekly heatmap on Overall live and static
status: done
priority: high
size: M
points: 5
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
tags: [dashboard, frontend, overall, metrics]
created: 2026-08-29
updated: 2026-08-29T18:09:45Z
started_at: 2026-08-29T18:05:00Z
completed_at: 2026-08-29T18:09:45Z
---

# T-MM-86b800a6: Show weekly heatmap on Overall live and static

## Description

Mount the weekly points heatmap on the Overall view only, above the hierarchical tree, on both the live board and the static board app. Keep metric cards and the tree as they are. Do not put the heatmap on Work items / Changelog.

## Acceptance criteria

- [x] Overall (live `BoardScreen` and `StaticBoardApp`) shows the heatmap above the tree when `view=overall`
- [x] Other views do not show the heatmap
- [x] Tree search, hide-completed, timeframe, pagination, and expand/deep-link behavior are unchanged
- [x] A board with no done leaves still renders Overall without layout breakage

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:46:00Z | prompt | Marco Mendão | Add an 8StarLabs-style heatmap on Overall for story points completed per week, in the board’s retro style, with strong UI/UX. |
| 2026-08-29T18:05:00Z | prompt | Marco Mendão | /tkmd-do S-MM-225ab050 and S-MM-2d3bf631 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T18:09:30Z | 2026-08-29T18:09:45Z | Mount heatmap on Overall live and static; keep it off Work items and Changelog. |
