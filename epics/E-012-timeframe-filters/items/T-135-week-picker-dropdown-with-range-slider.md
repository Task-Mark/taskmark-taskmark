---
id: T-135
type: task
title: Week picker dropdown with optional range slider
status: done
priority: medium
size: M
size_source: suggested
size_basis: [velocity:similar]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
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
tags: [filters, timeframe, weeks, frontend, ui]
created: 2026-07-24
updated: 2026-07-24T16:49:37.998Z
started_at: 2026-07-24T16:19:29Z
completed_at: 2026-07-24T16:21:26Z
actual_ms: 117000
---

# T-135: Week picker dropdown with optional range slider

## Description

Replace the always-visible week slider with a week picker button (like the date picker). The dropdown lists weeks to select; a bottom action enables week-range mode, which swaps the button for the week slider defaulting to the current week and the two weeks before.

## Acceptance criteria

- [x] Week control is an icon button that opens a dropdown to pick a single week.
- [x] Dropdown bottom offers week-range selection.
- [x] Choosing week range replaces the button with the week slider.
- [x] Default week range is current ISO week and two weeks before (clamped within the year).
- [x] Single-week pick filters to that week; clear restores none.

## Notes

Follow-up polish on E-012.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T16:19:29Z | prompt | Marco Mendão | Week picker like date picker; bottom enables range → slider with current week and two weeks before |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T16:19:29Z | 2026-07-24T16:21:26Z | week picker dropdown; range mode swaps to slider with current−2..current default |
