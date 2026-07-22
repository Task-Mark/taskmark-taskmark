---
id: S-009
type: story
title: Ambiguous common-name resolution
status: done
priority: high
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 4
points_source: rolled_up
estimate_minutes: 60
actual_minutes: 64
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-003
epic: E-003
owner: ""
blocked: false
cancelled: false
tags: [architecture, multi-repo, ux]
created: 2026-07-21
updated: 2026-07-21T23:57:22Z
started_at: 2026-07-21T22:34:16Z
completed_at: 2026-07-21T22:36:51Z
---
# S-009: Ambiguous common-name resolution

## User story

As a developer in a multi-project workspace, when the shared project name is ambiguous, I want Taskmark to ask me for the board project name so we do not create a wrongly named `<…>-taskmark` folder.

## Acceptance criteria

- [x] Heuristics detect when a common prefix/name cannot be derived confidently (e.g. unrelated folder names, conflicting prefixes).
- [x] On ambiguity, the agent/tooling asks the user for the intended common project name before creating the dedicated folder.
- [x] The chosen name is persisted (e.g. in `REPOS.md` or a board config field) so later syncs do not re-ask unless missing.
- [x] Non-ambiguous cases still auto-derive `<common>-taskmark` without prompting.

## Tasks

- [T-024: Detect ambiguous common-name cases](items/T-024-detect-ambiguous-common-name.md)
- [T-025: Prompt user and persist board project name](items/T-025-prompt-persist-board-name.md)

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
| 1 | agent | 2026-07-21T21:32:51Z | 2026-07-21T22:36:51Z | auto-backfilled: velocity × points (missing work log) |
