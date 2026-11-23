---
id: S-093
type: story
title: Delete unused scripts, rules, hooks, commands, and skills
status: backlog
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 18
points_source: rolled_up
estimate_minutes: 180
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

# S-093: Delete unused scripts, rules, hooks, commands, and skills

## User story

As a plugin maintainer, I want dead Taskmark surface area gone so agents cannot resurrect INDEX sync, velocity, or the old command set.

## Acceptance criteria

- [ ] Skills that only served removed commands (start-work, complete-work, sync-status, velocity, overview, log-commits, update-work-item as a user command, etc.) are deleted or folded into tsmk-*.
- [ ] Scripts only used for README dashboard, INDEX, VELOCITY, calibrate, contributor README are deleted.
- [ ] Hooks/rules/commands that are unused after the four-command model are deleted.
- [ ] Website command reference matches the four commands.

## Tasks

- [T-299: Delete unused skills, commands, hooks, and rules](items/T-299-delete-unused-skills-commands-hooks-rules.md)
- [T-300: Delete unused plugin scripts](items/T-300-delete-unused-scripts.md)
- [T-301: Update website docs to the four commands](items/T-301-update-website-command-docs.md)

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
