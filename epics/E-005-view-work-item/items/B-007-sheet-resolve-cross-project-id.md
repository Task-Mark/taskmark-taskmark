---
id: B-007
type: bug
title: Sheet parent and breadcrumb resolve same id from another project
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-159, B-006]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 1
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
tags: [dashboard, frontend, sheet, routing, bug]
created: 2026-07-25
updated: 2026-07-27T05:18:44.416Z
started_at: 2026-07-25T10:43:07Z
completed_at: 2026-07-25T10:44:19Z
actual_ms: 72000
---
# B-007: Sheet parent and breadcrumb resolve same id from another project

## Description

When navigating to a parent via the sheet back control or hierarchy breadcrumb, `resolveWorkItemById` searches all configured boards and returns the first match for that id. With multiple projects sharing ids (e.g. both have `E-001`), the sheet can open the wrong project’s item.

## Repro steps

1. Configure two Taskmark projects that both have an item with the same id (e.g. `E-001`).
2. Open a child work item from project A in the detail sheet.
3. Click the parent back control or an ancestor breadcrumb crumb.

## Fix criteria

- [x] Parent / breadcrumb / in-sheet id navigation resolves only within the board of the currently open work item.
- [x] Shared `?item=` links prefer the active project board (not an arbitrary other project with the same id).
- [x] Opening a missing id on the scoped board shows the sheet error state (does not silently load another project’s item).

## Notes

- Root cause: `findWorkItemInProjects` first-match across all roots.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-25T10:43:07Z | prompt | Marco Mendão | Parent/breadcrumb opens same id from a different project |
| 2 | 2026-07-25T10:44:19Z | feedback | Marco Mendão | Scoped sheet id resolve to current/active board |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 5701242 | taskmark-frontend | 2026-07-25T11:45:05+01:00 | Marco Mendão | fix sheet resolve to active board |
| 6335bfa | taskmark-taskmark | 2026-07-25T11:45:05+01:00 | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-25T10:43:07Z | 2026-07-25T10:44:19Z | Scoped resolveWorkItemById to current/active board |
