---
id: S-008
type: story
title: Multi-project dedicated board repo
status: done
priority: high
size: L
size_source: suggested
size_basis: [T-020, T-021, T-022, T-023]
points: 8
points_source: suggested
estimate_minutes: 734
actual_minutes: 2
estimate_basis: [T-020, T-021, T-022, T-023]
session_cap_minutes: 480
parent: E-003
epic: E-003
owner: ""
blocked: false
cancelled: false
tags: [architecture, multi-repo, board-layout, git]
created: 2026-07-21
updated: 2026-07-21T22:41:00Z
started_at: 2026-07-21T22:34:16Z
completed_at: 2026-07-21T22:36:51Z
---

# S-008: Multi-project dedicated board repo

## User story

As a developer working across multiple git projects in one workspace, I want a dedicated sibling project named `<common_project_name>-taskmark` with its own git so the board is shared once instead of copied into every product repo.

## Acceptance criteria

- [x] Workspace with two or more git roots is classified as multi-project mode.
- [x] A sibling folder `<common_project_name>-taskmark` is created (or reused if present) beside the linked projects.
- [x] That folder is initialized as its own git repository (`git init`) when created.
- [x] The dedicated project **root is the board** (`INDEX.md`, `epics/` at `<common>-taskmark/` — no nested `taskmark/` folder).
- [x] Product repos listed in `REPOS.md` are linked for commit attribution but do not each hold a full board copy.
- [x] Agents treat the dedicated project as the single source of truth for board edits.

## Tasks

- [T-020: Derive common project name](items/T-020-derive-common-project-name.md)
- [T-021: Create sibling `-taskmark` project folder](items/T-021-create-sibling-taskmark-project.md)
- [T-022: Initialize git for dedicated Taskmark project](items/T-022-init-git-for-taskmark-project.md)
- [T-023: Canonical board without product-repo copies](items/T-023-canonical-board-no-product-copies.md)
- [B-002: Dedicated board repo must be flat (no nested taskmark/)](items/B-002-flat-board-repo-root.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T22:26:00Z | prompt | Create epic: single-project board inside project git; multi-project sibling `-taskmark` repo; create stories/tasks |
| 2 | 2026-07-21T22:41:00Z | feedback | Board root is <name>-taskmark (flat); no nested taskmark/ |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
