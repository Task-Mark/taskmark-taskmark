---
id: E-003
type: epic
title: Refactor Taskmark project structure
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 31
points_source: rolled_up
estimate_minutes: 443
actual_minutes: 496
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
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
tags: [architecture, multi-repo, plugin, board-layout]
created: 2026-07-21
updated: 2026-07-27T05:16:43.229Z
started_at: 2026-07-21T22:34:16Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 29760000
estimate_source: rolled_up
---
# E-003: Refactor Taskmark project structure

## Goal

Stop copying `taskmark/` into every product repo. Place the board where git ownership is clear: inside the sole project for single-repo workspaces, or in a dedicated sibling `<common_project_name>-taskmark` git project whose **root is the board** for multi-repo workspaces.

## Scope

- Single-folder / single-git workspaces: `taskmark/` lives inside that project and uses the project’s git history.
- Multi-folder / multi-git workspaces: create a sibling project named `<common_project_name>-taskmark` (ask the user when the common name is ambiguous).
- Initialize a new git repository for the dedicated multi-project Taskmark folder.
- Update plugin conventions, skills, scripts, and the always-apply rule to match the new model.
- Provide a migration path away from per-repo board copies.

## Out of scope

- Changing epic/story/task markdown schema or INDEX format beyond repo-layout docs.
- Frontend dashboard UI redesign (discovery may need follow-up once layout lands).
- Hosting or remotes for the new Taskmark git repo (local `git init` only unless later requested).

## Success metrics

- Single-repo workspaces never create a sibling Taskmark project; board commits land in the product repo.
- Multi-repo workspaces have exactly one canonical board at `<name>-taskmark/` **root** (no nested `taskmark/`) with its own `.git`.
- Agents no longer sync/copy `taskmark/` into every linked product repo.
- Ambiguous naming always prompts the user before creating the dedicated project.

## Stories

- [S-007: Single-project board placement](stories/S-007-single-project-board-placement/story.md)
- [S-008: Multi-project dedicated board repo](stories/S-008-multi-project-dedicated-board/story.md)
- [S-009: Ambiguous common-name resolution](stories/S-009-ambiguous-common-name/story.md)
- [S-010: Migrate plugin tooling to new layout](stories/S-010-migrate-plugin-tooling/story.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 9510b02 | taskmark-taskmark | 2026-07-21T22:42:00Z | Marco Mendão | add flat taskmark board |
| f742175 | taskmark-cursor | 2026-07-21T22:42:00Z | Marco Mendão | flatten multi-repo board layout |
| 4605512 | taskmark-frontend | 2026-07-21T22:42:00Z | Marco Mendão | remove nested taskmark board copy |
| 87ec6aa | taskmark-frontend | 2026-07-21T22:31:15Z | Marco Mendão | add e-003 project structure epic |
| 6962bd4 | taskmark-cursor | 2026-07-21T22:31:15Z | Marco Mendão | sync taskmark board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T14:20:51Z | 2026-07-21T14:36:51Z | auto-backfilled: rollup from children (missing/under-logged) |
| 2 | Marco Mendão | 2026-07-21T14:36:51Z | 2026-07-21T22:36:51Z | auto-backfilled: rollup from children (missing/under-logged) |
