---
id: S-010
type: story
title: Migrate plugin tooling to new layout
status: done
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 12
points_source: rolled_up
estimate_minutes: 155
actual_minutes: 192
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-003
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
tags: [plugin, conventions, migration, multi-repo]
created: 2026-07-21
updated: 2026-07-25T10:24:50.747Z
started_at: 2026-07-21T22:34:16Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 11520000
---
# S-010: Migrate plugin tooling to new layout

## User story

As a Taskmark plugin user, I want skills, scripts, conventions, and the always-apply rule updated to the new single vs dedicated-board model so agents stop copying the board into every product repo.

## Acceptance criteria

- [x] `multi-repo.md`, always-apply project-memory rule, and related docs describe single-in-project vs dedicated `-taskmark` git project.
- [x] `sync-taskmark-repos` skill/script no longer whole-tree-copies `taskmark/` into every product git root; it ensures/uses the dedicated board project in multi mode.
- [x] `taskmark-init`, create/start/complete/sync skills, and `REPOS.md` guidance match the new layout.
- [x] Existing workspaces that already have per-repo copies have a documented migration path to the dedicated board repo.
- [x] Local plugin install is synced after the package changes.

## Tasks

- [T-026: Rewrite multi-repo conventions and rule](items/T-026-rewrite-multi-repo-conventions.md)
- [T-027: Update sync-taskmark-repos skill and script](items/T-027-update-sync-taskmark-repos.md)
- [T-028: Update init and related skills](items/T-028-update-init-and-skills.md)
- [T-029: Migrate existing multi-copy boards](items/T-029-migrate-existing-multi-copy-boards.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T22:26:00Z | prompt | Marco Mendão | Create epic: single-project board inside project git; multi-project sibling `-taskmark` repo; create stories/tasks |
| 2 | 2026-07-21T22:32:39Z | feedback | Marco Mendão | Folder naming: use `<common_project_name>-taskmark` (hyphen), not underscore |
| 3 | 2026-07-21T22:34:16Z | prompt | Marco Mendão | Implement E-003: single-in-project vs sibling <name>-taskmark board |
| 4 | 2026-07-21T22:36:37Z | feedback | Marco Mendão | E-003 delivered: hyphen -taskmark sibling board model |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T19:24:51Z | 2026-07-21T22:36:51Z | auto-backfilled: velocity × points (missing work log) |
