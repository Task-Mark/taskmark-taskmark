---
id: T-MM-9d1037cd
type: task
title: Retro weekly heatmap component
status: done
priority: high
size: L
points: 8
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
tags: [frontend, overall, ux, metrics]
created: 2026-08-29
updated: 2026-08-29T18:36:00Z
started_at: 2026-08-29T18:05:00Z
completed_at: 2026-08-29T18:09:45Z
---

# T-MM-9d1037cd: Retro weekly heatmap component

## Description

Implement a contribution-calendar heatmap (weeks as columns, one square per week — not seven daily cells with a weekly total). Match the board’s retro / neo-brutalist language: thick borders, hard offset shadows, a short discrete color scale from empty to high, month labels, and a small legend. Tooltips and keyboard focus must state the ISO week range and point count. Prefer a first-party component over copying the 8StarLabs package so colors and chrome stay on-brand.

## Acceptance criteria

- [x] Layout reads as a GitHub/8StarLabs-style calendar of weeks with month labels and a low-to-high legend
- [x] Each cell is one ISO week; color intensity maps to that week’s story-point total; zero weeks stay visually empty
- [x] Styling matches existing metric cards (hard black border, offset shadow, board palette) in light and dark themes
- [x] Hover and keyboard focus show week range and “N story points” (or equivalent); screen readers get a concise summary of the series
- [x] Horizontal overflow scrolls without clipping labels; cells remain tappably large on a typical phone width
- [x] Empty series (all zeros) still shows the grid and an honest empty message, not a broken chart

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:46:00Z | prompt | Marco Mendão | Add an 8StarLabs-style heatmap on Overall for story points completed per week, in the board’s retro style, with strong UI/UX. |
| 2026-08-29T18:05:00Z | prompt | Marco Mendão | /tkmd-do S-MM-225ab050 and S-MM-2d3bf631 |
| 2026-08-29T18:20:00Z | feedback | Marco Mendão | The heatmap must show a full year like a GitHub calendar (day cells, weekday and month labels) and use shades of #C4A1FF only, white for zero. |
| 2026-08-29T18:28:00Z | feedback | Marco Mendão | The heatmap should be centred inside its card. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T18:08:45Z | 2026-08-29T18:09:30Z | Retro weekly heatmap component with legend, tooltips, and empty-state copy. |
| Marco Mendão | 2026-08-29T18:20:00Z | 2026-08-29T18:32:00Z | Rebuilt as a one-year day calendar with a white-to-#C4A1FF scale. |
| Marco Mendão | 2026-08-29T18:33:00Z | 2026-08-29T18:36:00Z | Centred the calendar and legend inside the card while keeping narrow-screen scrolling. |
