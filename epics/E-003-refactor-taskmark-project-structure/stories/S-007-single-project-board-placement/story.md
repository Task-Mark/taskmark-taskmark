---
id: S-007
type: story
title: Single-project board placement
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 74
actual_minutes: 80
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-003
epic: E-003
owner: ""
blocked: false
cancelled: false
tags: [architecture, single-repo, board-layout]
created: 2026-07-21
updated: 2026-07-23T15:41:41.235Z
started_at: 2026-07-21T22:34:16Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 4800000
---
# S-007: Single-project board placement

## User story

As a developer with a single-folder / single-git workspace, I want the Taskmark board to live inside that project and use its git so product memory stays with the code without a separate Taskmark repo.

## Acceptance criteria

- [x] Workspace with exactly one git root is classified as single-project mode.
- [x] `taskmark/` is created or expected only under that git root (not a sibling folder).
- [x] Board commits and history use the project’s existing git repository.
- [x] `REPOS.md` lists that single project; no multi-repo copy sync is required.
- [x] Docs/skills describe single-project placement clearly.

## Tasks

- [T-017: Detect single-repo workspace mode](items/T-017-detect-single-repo-mode.md)
- [T-018: Place board inside project git root](items/T-018-place-board-in-project-git.md)
- [T-019: Configure single-repo REPOS.md](items/T-019-single-repo-repos-md.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T22:26:00Z | prompt | Create epic: single-project board inside project git; multi-project sibling `-taskmark` repo; create stories/tasks |
| 2 | 2026-07-21T22:32:39Z | feedback | Folder naming: use `<common_project_name>-taskmark` (hyphen), not underscore |
| 3 | 2026-07-21T22:34:16Z | prompt | Implement E-003: single-in-project vs sibling <name>-taskmark board |
| 4 | 2026-07-21T22:36:37Z | feedback | E-003 delivered: hyphen -taskmark sibling board model |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T21:16:51Z | 2026-07-21T22:36:51Z | auto-backfilled: velocity × points (missing work log) |
