---
id: T-008
type: task
title: Discover Taskmark projects under master folder
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 3
estimate_basis: [calibrated:T-008]
session_cap_minutes: 480
parent: S-001
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
tags: [mvp, discovery, filesystem]
created: 2026-07-21
updated: 2026-07-24T16:57:53.518Z
started_at: 2026-07-21T16:35:18Z
completed_at: 2026-07-21T16:37:18Z
actual_ms: 180000
---

# T-008: Discover Taskmark projects under master folder

## Description

Given a selected **master folder**, walk its subfolders to find configured Taskmark boards (`taskmark/` with expected markers such as `INDEX.md` and/or `epics/`). Return a list of discovered projects (name/path) so the app can treat the master folder as a workspace that may contain **multiple** Taskmark projects—not a single board at the root.

## Acceptance criteria

- [x] Scans subfolders of the master folder for Taskmark boards (at least one level deep; document depth policy).
- [x] Returns zero or more project entries with a stable id/name and absolute path to each board root.
- [x] Skips noise (e.g. `node_modules`, `.git`) so discovery stays practical.
- [x] A master folder with several git/project subfolders each containing `taskmark/` yields multiple discoveries (e.g. this workspace’s `taskmark-frontend` and `taskmark-cursor`).
- [x] Does not require `taskmark/` to exist at the master folder root itself.

## Notes

Example: master `/Users/.../taskmark` → discover `/Users/.../taskmark/taskmark-frontend/taskmark` and `/Users/.../taskmark/taskmark-cursor/taskmark`.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T16:31:04Z | feedback | Marco Mendão | Master folder may contain multiple Taskmark projects in subfolders; discover by venturing into children |
| 2 | 2026-07-21T16:37:18Z | prompt | Marco Mendão | Implement S-001 setup wizard |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T15:49:18Z | 2026-07-21T15:52:18Z | auto-backfilled: velocity × points (missing work log); shared-batch: 3 of 6min by points |
