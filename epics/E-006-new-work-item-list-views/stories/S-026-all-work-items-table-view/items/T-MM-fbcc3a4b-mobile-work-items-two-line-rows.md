---
id: T-MM-fbcc3a4b
type: task
title: Stack Work items rows on mobile with title then metadata
status: done
priority: high
size: M
points: 5
parent: S-026
epic: E-006
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
tags: [dashboard, frontend, views, mobile, ux]
created: 2026-09-01
updated: 2026-09-01T06:48:49Z
started_at: 2026-09-01T06:13:26Z
completed_at: 2026-09-01T06:17:26Z
---

# T-MM-fbcc3a4b: Stack Work items rows on mobile with title then metadata

## Description

The Work items tab is a nine-column table that only fits on a phone by scrolling sideways. Below `sm`, replace that table with stacked rows: the work-item title first, then ID, type, epic, size, people, priority, and status/progress on a wrapping metadata line. Keep the current sortable table from `sm` upward. Expose the same sort keys on mobile through a compact control so sorting is not lost when headers are hidden.

## Acceptance criteria

- [x] Below `sm`, Work items shows stacked rows (title, then metadata) with no horizontal scroll
- [x] All current fields remain available: ID, type, title, epic, size, people, priority, and status or story progress
- [x] A compact mobile sort control uses the same sort state as the desktop table headers
- [x] Filters, pagination, and opening item detail still work
- [x] The desktop table is unchanged from `sm` upward

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-01T06:12:00Z | prompt | Marco Mendão | From a Cursor plan: on mobile, Overall and Work items rows should show the work-item name first and other information underneath. |
| 2026-09-01T06:13:26Z | prompt | Marco Mendão | /tkmd-save-do: implement the mobile two-line Work items rows. |
| 2026-09-01T06:28:00Z | feedback | Marco Mendão | On mobile show a done/total count instead of the progress bar and align the epic tag with the title. |
| 2026-09-01T06:36:14Z | feedback | Marco Mendão | Row buttons must sit vertically centred across both mobile lines. |
| 2026-09-01T06:42:56Z | feedback | Marco Mendão | Make the view button and caret a bit smaller so work-item information has more prominence. |
| 2026-09-01T06:48:49Z | feedback | Marco Mendão | On mobile the work-item name must stay on a single line, clipping with an ellipsis when needed. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-01T06:13:26Z | 2026-09-01T06:17:26Z | Stacked Work items mobile rows plus a compact sort control sharing desktop sort state. |
| Marco Mendão | 2026-09-01T06:20:00Z | 2026-09-01T06:36:14Z | Mobile row wraps both text lines in one column so the view button stays vertically centred, with epic tag inline and a done/total count. |
| Marco Mendão | 2026-09-01T06:42:56Z | 2026-09-01T06:42:56Z | Shrunk the mobile view button so title and metadata take more of the row. |
| Marco Mendão | 2026-09-01T06:48:00Z | 2026-09-01T06:48:49Z | Mobile titles now truncate to one line beside the epic tag, with the full text kept as a tooltip. |
