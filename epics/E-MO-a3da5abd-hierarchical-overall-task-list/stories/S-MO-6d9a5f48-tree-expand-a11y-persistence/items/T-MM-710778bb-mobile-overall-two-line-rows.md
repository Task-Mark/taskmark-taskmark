---
id: T-MM-710778bb
type: task
title: Stack Overall tree rows on mobile with title then metadata
status: done
priority: high
size: M
points: 5
parent: S-MO-6d9a5f48
epic: E-MO-a3da5abd
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
tags: [dashboard, frontend, overall, mobile, ux]
created: 2026-09-01
updated: 2026-09-01T06:48:49Z
started_at: 2026-09-01T06:13:26Z
completed_at: 2026-09-01T06:17:26Z
---

# T-MM-710778bb: Stack Overall tree rows on mobile with title then metadata

## Description

On phone widths the Overall tree still packs identity, status, and the view action into an awkward two-column grid, then puts the view button on a third strip. Follow up on the existing indent and touch-target work so each node reads as two zones: the title (with expand and view) first, then compact metadata underneath. Desktop column layout stays unchanged.

```
[expand] Title text                    [view]
ID  type  size  people  items  status
```

## Acceptance criteria

- [x] Below `sm`, each tree node shows the title on the first line and remaining metadata on a second wrapping line
- [x] Expand, view, keyboard, `aria-expanded`, indent, selection, and session expand persistence still work
- [x] Size, people, item count, and status/progress remain visible on mobile without horizontal scroll
- [x] Desktop Overall grid and column headers stay as they are from `sm` upward

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-01T06:12:00Z | prompt | Marco Mendão | From a Cursor plan: on mobile, Overall and Work items rows should show the work-item name first and other information underneath. |
| 2026-09-01T06:13:26Z | prompt | Marco Mendão | /tkmd-save-do: implement the mobile two-line Overall tree rows. |
| 2026-09-01T06:28:00Z | feedback | Marco Mendão | On mobile drop the progress bar for a plain done/total count and remove the "items" label. |
| 2026-09-01T06:36:14Z | feedback | Marco Mendão | Row buttons must sit vertically centred across both mobile lines. |
| 2026-09-01T06:42:56Z | feedback | Marco Mendão | Make the view button and caret a bit smaller so work-item information has more prominence. |
| 2026-09-01T06:48:49Z | feedback | Marco Mendão | On mobile the work-item name must stay on a single line, clipping with an ellipsis when needed. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-01T06:13:26Z | 2026-09-01T06:17:26Z | Stacked Overall mobile rows: title with expand and view, metadata wrapping underneath. |
| Marco Mendão | 2026-09-01T06:20:00Z | 2026-09-01T06:36:14Z | Mobile rows now use a three-column grid so expand and view stay centred across both lines, with a done/total count instead of the progress bar. |
| Marco Mendão | 2026-09-01T06:42:56Z | 2026-09-01T06:42:56Z | Shrunk the mobile expand caret and view button so title and metadata take more of the row. |
| Marco Mendão | 2026-09-01T06:48:00Z | 2026-09-01T06:48:49Z | Mobile tree titles now truncate to one line, with the full text kept as a tooltip. |
