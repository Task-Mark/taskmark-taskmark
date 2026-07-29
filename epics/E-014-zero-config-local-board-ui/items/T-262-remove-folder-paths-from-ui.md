---
id: T-262
type: task
title: Remove folder path references from board UI
status: done
priority: medium
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 4
estimate_source: suggested
estimate_basis: [calibrated:T-262]
session_cap_minutes: 480
parent: E-014
epic: E-014
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
tags: [frontend, ui, privacy]
created: 2026-07-29
updated: 2026-07-29T07:31:14.976Z
started_at: 2026-07-29T07:08:36Z
completed_at: 2026-07-29T07:13:00Z
actual_ms: 240000
---
# T-262: Remove folder path references from board UI

## Description

Stop showing absolute filesystem paths in the board UI (for example `/Users/menda0/Projects/taskmark/taskmark-taskmark`). Users should not see machine-local folder paths in chrome, labels, or secondary copy.

## Acceptance criteria

- [x] No absolute folder paths are displayed in the board UI chrome or primary surfaces.
- [x] Where a board/project identity is needed, use a friendly name (e.g. board/project title or short name) instead of a path.
- [x] Spot-check setup, app bar, board header, and any status/detail areas that previously echoed paths.

## Notes

Example of what must not appear: `/Users/menda0/Projects/taskmark/taskmark-taskmark`.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-29T05:50:53Z | prompt | Marco Mendão | Remove all folder path references from UI (e.g. absolute board path) |
| 2 | 2026-07-29T07:08:36Z | prompt | Marco Mendão | implement T-260, T-261 and T-262 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T07:08:36Z | 2026-07-29T07:12:36Z | shared-batch: 2 of 4min by points — Remove absolute paths from chrome, lists, errors |
