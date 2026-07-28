---
id: E-012
type: epic
title: Timeframe filters for solved work items
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 39
points_source: rolled_up
estimate_minutes: 545
actual_minutes: 15
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
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
tags: [dashboard, frontend, lists, filters, timeframe]
created: 2026-07-23
updated: 2026-07-28T06:20:01.202Z
started_at: 2026-07-24T16:02:37Z
completed_at: 2026-07-27T07:06:27Z
actual_ms: 946000
---

# E-012: Timeframe filters for solved work items

## Goal

Let users narrow epics, stories, tasks, and bugs to those **solved** in a chosen timeframe — either by year + week numbers (slider), or by an explicit date range — so delivery history is easy to review by period.

## Scope

- Year dropdown populated from years present on the board (`completed_at`); if only one year exists, hide the year control and show week numbers only.
- Week-number range slider for the selected (or sole) year; show only items solved in those ISO weeks.
- Date range picker (from → to); show only items solved within that inclusive range.
- Apply to Overall epic/story/task lists and Work items list (and epic-level drill-down as applicable).
- Compose with existing search, hide-completed, parent/tag filters, and pagination (reset page on change).

## Out of scope

- Filtering by `created` / `started_at` (solved/`completed_at` only for v1).
- Saving timeframe presets or syncing filters to the URL (optional later).
- Server-side indexing.

## Success metrics

- User can pick year+weeks or a date range and see only work items with `completed_at` in that window.
- Single-year boards show week slider without a year dropdown.
- Empty results show a clear empty state; clearing the timeframe restores the unfiltered list.

## Stories

- [S-044: Shared timeframe filter plumbing](stories/S-044-shared-timeframe-filter-plumbing/story.md)
- [S-045: Year and week number filter](stories/S-045-year-and-week-number-filter/story.md)
- [S-046: Date range picker filter](stories/S-046-date-range-picker-filter/story.md)

## Tasks

- [T-134: Move timeframe controls to card header](items/T-134-move-timeframe-controls-to-card-header.md)
- [T-135: Week picker dropdown with optional range slider](items/T-135-week-picker-dropdown-with-range-slider.md)
- [T-136: Highlight and quick-select current week in picker](items/T-136-highlight-current-week-in-picker.md)
- [T-137: Mark prev/next weeks and widen week slider](items/T-137-mark-prev-next-weeks-widen-slider.md)
- [T-138: Scroll week picker to current week; distinct prev/next colors](items/T-138-scroll-to-current-week-distinct-colors.md)
- [T-139: Week/day completion counts and prev/next opacity](items/T-139-week-day-completion-counts-opacity.md)
- [T-140: Week range dual dropdown instead of slider](items/T-140-week-range-dual-dropdown.md)

- [T-180: Show story points per day on calendar picker](items/T-180-calendar-day-story-points.md)

- [T-181: Align calendar points with leaf speed logic](items/T-181-align-calendar-points-with-leaf-speed.md)

- [T-182: Compact calendar point badges](items/T-182-compact-calendar-point-badges.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| d5f8f02 | taskmark-frontend | 2026-07-27T07:08:31Z | Marco Mendão | add project metrics and calendar points |
| d010f70 | taskmark-frontend | 2026-07-24T17:00:20Z | Marco Mendão | use dual week dropdown for range filter |
| efa533f | taskmark-taskmark | 2026-07-24T17:00:20Z | Marco Mendão | complete t-140 week range dual dropdown |
| f85e61c | taskmark-frontend | 2026-07-24T16:54:00Z | Marco Mendão | add timeframe filters for solved work items |
| ea2c152 | taskmark-taskmark | 2026-07-24T16:54:00Z | Marco Mendão | complete e-012 timeframe filters |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-24T16:02:37Z | 2026-07-24T16:02:37Z | rollup: children hold shared-batch; delivered E-012 timeframe filters for solved work items |
