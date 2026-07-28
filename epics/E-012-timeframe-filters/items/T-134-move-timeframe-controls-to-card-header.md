---
id: T-134
type: task
title: Move timeframe controls to card header
status: done
priority: medium
size: S
size_source: suggested
size_basis: [velocity:similar]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
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
tags: [filters, timeframe, frontend, ui]
created: 2026-07-24
updated: 2026-07-28T08:37:10.649Z
started_at: 2026-07-24T16:14:35Z
completed_at: 2026-07-24T16:15:29Z
actual_ms: 54000
---
# T-134: Move timeframe controls to card header

## Description

Place the week slider and date-range control on the top right of each list card, aligned with the card title. Date range is an icon-only button (no label).

## Acceptance criteria

- [x] Date range control is an icon button with no visible label (accessible name via aria-label).
- [x] Week slider and date range sit in the card header top-right, aligned with the title.
- [x] Applies to epic, story, task, and work-items list cards.

## Notes

Follow-up polish on E-012.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T16:14:35Z | prompt | Marco Mendão | Date range icon-only; week slider + date range top-right of card aligned with title |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T16:14:35Z | 2026-07-24T16:15:29Z | moved week slider + date icon to card header (CardAction) |
