---
id: T-161
type: task
title: In-sheet back button for detail navigation
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-159, T-049]
points: 2
points_source: suggested
estimate_minutes: 30
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
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [dashboard, frontend, sheet, detail, routing]
created: 2026-07-25
updated: 2026-07-27T06:17:22.249Z
started_at: 2026-07-25T10:23:49Z
completed_at: 2026-07-25T10:24:34Z
actual_ms: 45000
---
# T-161: In-sheet back button for detail navigation

## Description

When the user navigates from one work item detail sheet to another (child, parent, or related link), show a Back control on the sheet so they can return to the previous item without relying only on the browser chrome.

## Acceptance criteria

- [x] After navigating from detail A to detail B inside the sheet, a Back control is visible.
- [x] Activating Back returns to the previous work item detail (A) and updates the URL accordingly.
- [x] Back is hidden when there is no prior in-sheet detail (first open from a list or shared link).
- [x] Closing the sheet clears the in-sheet back stack.

## Notes

- Builds on T-159 URL history (`?item=` pushes).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-25T10:23:49Z | prompt | Marco Mendão | If navigating sheet to sheet, show a back button to return |
| 2 | 2026-07-25T10:24:34Z | feedback | Marco Mendão | In-sheet back button shipped |
| 3 | 2026-07-25T10:27:26Z | prompt | Marco Mendão | Back = icon + work item code only; align left with sheet title |
| 4 | 2026-07-25T10:30:27Z | prompt | Marco Mendão | Back icon align with X; work item code = hierarchy breadcrumb |
| 5 | 2026-07-25T10:33:04Z | prompt | Marco Mendão | Align back with X; arrow goes to parent work item |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| b66202d | taskmark-frontend | 2026-07-25T11:34:33+01:00 | Marco Mendão | add detail sheet routes and overall work items |
| 861fc90 | taskmark-taskmark | 2026-07-25T11:34:33+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-25T10:23:49Z | 2026-07-25T10:24:34Z | Added in-sheet Back control with navigation stack |
