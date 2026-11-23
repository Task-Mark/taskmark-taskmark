---
id: R-timeframe-filters-for-solved-work-items
type: request
title: Timeframe filters for solved work items
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-23
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - dashboard
  - frontend
  - lists
  - filters
  - timeframe
aliases:
  - E-012
source_meetings: []
links: []
---

# Timeframe filters for solved work items

## Goal

Let users narrow epics, stories, tasks, and bugs to those **solved** in a chosen timeframe — either by year + week numbers (slider), or by an explicit date range — so delivery history is easy to review by period.

## Scope

- Year dropdown populated from years present on the board (`completed_at`); if only one year exists, hide the year control and show week numbers only.
- Week-number range slider for the selected (or sole) year; show only items solved in those ISO weeks.
- Date range picker (from → to); show only items solved within that inclusive range.
- Apply to Overall epic/story/task lists and Work items list (and epic-level drill-down as applicable).
- Compose with existing search, hide-completed, parent/tag filters, and pagination (reset page on change).

## Done when

- User can pick year+weeks or a date range and see only work items with `completed_at` in that window.
- Single-year boards show week slider without a year dropdown.
- Empty results show a clear empty state; clearing the timeframe restores the unfiltered list.

## Out of scope

- Filtering by `created` / `started_at` (solved/`completed_at` only for v1).
- Saving timeframe presets or syncing filters to the URL (optional later).
- Server-side indexing.

## Open questions

_None yet._
