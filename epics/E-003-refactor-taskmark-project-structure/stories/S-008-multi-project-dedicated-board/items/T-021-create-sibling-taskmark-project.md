---
id: T-021
type: task
title: Create sibling `-taskmark` project folder
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-018, T-008]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_basis: [calibrated:T-021]
session_cap_minutes: 480
parent: S-008
epic: E-003
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
tags: [architecture, multi-repo, init]
created: 2026-07-21
updated: 2026-07-28T07:41:00.094Z
started_at: 2026-07-21T22:04:51Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 0
---

# T-021: Create sibling `-taskmark` project folder

## Description

In multi-project mode, create (or reuse) a sibling directory named `<common_project_name>-taskmark` next to the linked product projects. That directory’s **root is the board** (no nested `taskmark/` folder).

## Acceptance criteria

- [x] Folder path is sibling to product repos (not nested inside one of them).
- [x] Name follows `<common>-taskmark` from T-020 / T-025.
- [x] Existing folder with a valid board is reused, not duplicated.
- [x] Fresh folder gets `taskmark-init` content at the **repo root** (`INDEX.md`, `epics/`, … — not under a nested `taskmark/`).

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T22:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for Taskmark project structure refactor |
| 2 | 2026-07-21T22:32:39Z | feedback | Marco Mendão | Folder naming: use `<common_project_name>-taskmark` (hyphen), not underscore |
| 3 | 2026-07-21T22:36:37Z | feedback | Marco Mendão | E-003 delivered: hyphen -taskmark sibling board model |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T22:04:51Z | 2026-07-21T22:04:51Z | auto-backfilled: velocity × points (missing work log); shared-batch: 0 of 1min by points |
