---
id: T-159
type: task
title: Materialized detail sheet route with back navigation
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-083, T-049, T-069]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 3
estimate_source: suggested
estimate_basis: [calibrated:T-159]
session_cap_minutes: 480
parent: E-005
epic: E-005
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
tags: [dashboard, frontend, sheet, detail, routing]
created: 2026-07-24
updated: 2026-07-28T15:03:07.151Z
started_at: 2026-07-25T10:18:40Z
completed_at: 2026-07-25T10:22:08Z
actual_ms: 208000
---

# T-159: Materialized detail sheet route with back navigation

## Description

Make the work item detail sheet a materialized URL so users can navigate to it, bookmark it, and share a link that reopens the same item in the sheet. Keep the sheet presentation (not a full-page replacement of the board).

When the user opens another work item from inside a detail sheet (e.g. a child or parent), push history so browser Back returns to the previous work item detail rather than closing the sheet or jumping only to the list.

## Acceptance criteria

- [x] Opening a work item detail updates the URL to a stable, shareable route (or query) that identifies the item (id and/or path).
- [x] Loading / pasting that URL with a valid item opens the detail sheet for that item on the board.
- [x] Closing the sheet clears the detail from the URL and leaves the user on the underlying list/board context.
- [x] Navigating from one work item detail to another (child list, parent link, or similar in-sheet links) pushes history so Back restores the previous item’s detail sheet.
- [x] Invalid or missing item ids show the existing sheet empty/error state without breaking the board route.
- [x] Sheet UI remains a sheet over the board (not a separate full-page-only detail view).

## Notes

- Prefer URL state that works with the existing Next.js board route and `WorkItemSheetProvider`.
- E-005 originally listed separate full-page detail routes as out of scope; this task keeps the sheet UX and only materializes navigation/shareability.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:32:54Z | prompt | Marco Mendão | Sheet details as materialized route for share/nav; Back between work item details |
| 2 | 2026-07-25T10:18:40Z | prompt | Marco Mendão | implement this T-159 |
| 3 | 2026-07-25T10:22:08Z | feedback | Marco Mendão | Materialized detail sheet route implemented |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| b66202d | taskmark-frontend | 2026-07-25T11:34:33+01:00 | Marco Mendão | add detail sheet routes and overall work items |
| 861fc90 | taskmark-taskmark | 2026-07-25T11:34:33+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-25T10:18:40Z | 2026-07-25T10:22:08Z | Materialized ?item= URL for sheet; push history for in-sheet nav; back restores prior detail |
