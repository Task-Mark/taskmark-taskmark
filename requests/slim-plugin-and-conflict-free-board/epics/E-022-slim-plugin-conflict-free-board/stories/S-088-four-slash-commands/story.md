---
id: S-088
type: story
title: Only four user-facing slash commands
status: backlog
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 47
points_source: rolled_up
estimate_minutes: 470
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-022
epic: E-022
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, collaboration, board]
created: 2026-08-28
updated: 2026-08-28T12:37:43.783Z
started_at: null
completed_at: null
actual_ms: 0
---

# S-088: Only four user-facing slash commands

## User story

As a Cursor user, I want only `/tsmk-init`, `/tsmk-create`, `/tsmk-commit`, and `/tsmk-do` so that the plugin is simple and `/tsmk-do` never commits.

## Acceptance criteria

- [ ] Plugin command palette exposes exactly those four commands (plus none of the old `/new-*`, `/sync-*`, `/complete-work`, `/velocity`, etc.).
- [ ] `/tsmk-create` can create an epic, a story, a task/bug, or a whole tree from a prose description.
- [ ] `/tsmk-do` implements work, never runs git commit/commit-all, skips `in_progress`, and marks executed leaves `done` before the agent stops.
- [ ] `/tsmk-commit` is the only command that commits linked projects.
- [ ] `/tsmk-init` remains the board bootstrap path.

## Tasks

- [T-279: Add /tsmk-init command and skill](items/T-279-add-tsmk-init.md)
- [T-280: Add /tsmk-create for epic, story, task, or tree](items/T-280-add-tsmk-create.md)
- [T-281: Add /tsmk-commit for multi-repo commits](items/T-281-add-tsmk-commit.md)
- [T-282: Add /tsmk-do implement without commit or in_progress](items/T-282-add-tsmk-do.md)
- [T-283: Delete all other slash commands](items/T-283-remove-old-slash-commands.md)
- [T-284: Rewrite always-apply rules for the four-command model](items/T-284-rewrite-rules-for-four-commands.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-28T12:19:14Z | prompt | Marco Mendão | Full housekeeping: slim commands, drop derived board files, static sizing, leaf-only MD, new IDs, delete unused plugin pieces. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
