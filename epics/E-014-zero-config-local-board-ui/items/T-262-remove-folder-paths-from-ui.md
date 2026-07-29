---
id: T-262
type: task
title: Remove folder path references from board UI
status: backlog
priority: medium
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:14min/pt]
session_cap_minutes: 480
parent: E-014
epic: E-014
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, ui, privacy]
created: 2026-07-29
updated: 2026-07-29T06:48:27.505Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-262: Remove folder path references from board UI

## Description

Stop showing absolute filesystem paths in the board UI (for example `/Users/menda0/Projects/taskmark/taskmark-taskmark`). Users should not see machine-local folder paths in chrome, labels, or secondary copy.

## Acceptance criteria

- [ ] No absolute folder paths are displayed in the board UI chrome or primary surfaces.
- [ ] Where a board/project identity is needed, use a friendly name (e.g. board/project title or short name) instead of a path.
- [ ] Spot-check setup, app bar, board header, and any status/detail areas that previously echoed paths.

## Notes

Example of what must not appear: `/Users/menda0/Projects/taskmark/taskmark-taskmark`.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-29T05:50:53Z | prompt | Marco Mendão | Remove all folder path references from UI (e.g. absolute board path) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
