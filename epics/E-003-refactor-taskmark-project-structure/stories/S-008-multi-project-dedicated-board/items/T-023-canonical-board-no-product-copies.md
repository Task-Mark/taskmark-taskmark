---
id: T-023
type: task
title: Canonical board without product-repo copies
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-007, T-005]
points: 3
points_source: suggested
estimate_minutes: 480
actual_minutes: 0
estimate_basis: []
session_cap_minutes: 480
parent: S-008
epic: E-003
owner: ""
blocked: false
cancelled: false
tags: [architecture, multi-repo, canonical]
created: 2026-07-21
updated: 2026-07-21T23:18:07Z
started_at: null
completed_at: 2026-07-21T22:36:51Z
---
# T-023: Canonical board without product-repo copies

## Description

Make the dedicated `-taskmark` project the only board location in multi-project mode — board files at that repo’s **root**. `REPOS.md` still lists product git roots for commit attribution, but agents must not keep or sync board copies inside those product repos.

## Acceptance criteria

- [x] Canonical path is the dedicated Taskmark project **root** (not a nested `taskmark/` folder).
- [x] Product repos are listed in `REPOS.md` without requiring a local `taskmark/` copy.
- [x] Sync behavior no longer overwrites product repos with board trees.
- [x] Commits log still records product-repo SHAs with correct Repo names.

## Notes

Replaces the current “copy board into every git root” model.

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T22:26:00Z | prompt | Create epic + stories/tasks for Taskmark project structure refactor |
| 2 | 2026-07-21T22:36:37Z | feedback | E-003 delivered: hyphen -taskmark sibling board model |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
