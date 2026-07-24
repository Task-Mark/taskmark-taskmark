---
id: T-159
type: task
title: Materialized detail sheet route with back navigation
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-083, T-049, T-069]
points: 3
points_source: suggested
estimate_minutes: 45
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
session_cap_minutes: 480
parent: E-005
epic: E-005
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, sheet, detail, routing]
created: 2026-07-24
updated: 2026-07-24T17:39:50.198Z
started_at: null
completed_at: null
actual_ms: 0
---
# T-159: Materialized detail sheet route with back navigation

## Description

Make the work item detail sheet a materialized URL so users can navigate to it, bookmark it, and share a link that reopens the same item in the sheet. Keep the sheet presentation (not a full-page replacement of the board).

When the user opens another work item from inside a detail sheet (e.g. a child or parent), push history so browser Back returns to the previous work item detail rather than closing the sheet or jumping only to the list.

## Acceptance criteria

- [ ] Opening a work item detail updates the URL to a stable, shareable route (or query) that identifies the item (id and/or path).
- [ ] Loading / pasting that URL with a valid item opens the detail sheet for that item on the board.
- [ ] Closing the sheet clears the detail from the URL and leaves the user on the underlying list/board context.
- [ ] Navigating from one work item detail to another (child list, parent link, or similar in-sheet links) pushes history so Back restores the previous item’s detail sheet.
- [ ] Invalid or missing item ids show the existing sheet empty/error state without breaking the board route.
- [ ] Sheet UI remains a sheet over the board (not a separate full-page-only detail view).

## Notes

- Prefer URL state that works with the existing Next.js board route and `WorkItemSheetProvider`.
- E-005 originally listed separate full-page detail routes as out of scope; this task keeps the sheet UX and only materializes navigation/shareability.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:32:54Z | prompt | Marco Mendão | Sheet details as materialized route for share/nav; Back between work item details |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
