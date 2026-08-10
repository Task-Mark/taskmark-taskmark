---
id: T-006
type: task
title: Build epic list UI
status: done
priority: high
size: XS
size_source: suggested
size_basis: [calibrated:T-006]
points: 1
points_source: suggested
estimate_minutes: 45
actual_minutes: 47
estimate_basis: [calibrated:T-006]
session_cap_minutes: 480
parent: S-002
epic: E-001
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
tags: [mvp, epics, ui]
created: 2026-07-21
updated: 2026-07-29T11:30:07.936Z
started_at: 2026-07-21T16:49:52Z
completed_at: 2026-07-21T16:51:19Z
actual_ms: 2828000
---

# T-006: Build epic list UI

## Description

Build the epics list view using existing table/UI primitives: show every epic for **each** discovered project under the master folder, with project identity (name/path) plus id, title, status, size, points, and estimate/actual minutes. Include loading and empty states (no projects, or projects with no epics).

## Acceptance criteria

- [x] Renders a list/table of epics with the core summary columns.
- [x] Epics are grouped or labeled by discovered project.
- [x] Empty board / no projects shows a helpful empty state.
- [x] Loading and error states are distinct.
- [x] Uses project UI components (e.g. table) where appropriate.

## Notes

Story/task drill-down is out of scope for this MVP slice.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 3 | 2026-07-21T16:51:19Z | prompt | Marco Mendão | Implement S-002 epic list |
| 1 | 2026-07-21T16:24:55Z | prompt | Marco Mendão | Create MVP epic with setup wizard + epic list; create stories and tasks |
| 2 | 2026-07-21T16:31:04Z | feedback | Marco Mendão | List epics per project discovered under master folder |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 3d64d0e | taskmark-frontend | 2026-07-21T17:35:33Z | Marco Mendão | format epic list durations and status badges |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T16:49:52Z | 2026-07-21T16:51:19Z | Built per-project epic list table UI |
| 2 | Marco Mendão | 2026-07-21T16:49:52Z | 2026-07-21T17:35:33Z | auto-recovered: commit span |
