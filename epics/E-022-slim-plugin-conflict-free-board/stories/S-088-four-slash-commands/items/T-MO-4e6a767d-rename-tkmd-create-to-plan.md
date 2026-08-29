---
id: T-MO-4e6a767d
type: task
title: Rename /tkmd-create to /tkmd-plan
status: backlog
priority: high
size: M
points: 5
parent: S-088
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, commands, planning]
created: 2026-08-29
updated: 2026-08-29T10:39:07Z
started_at: null
completed_at: null
---

# T-MO-4e6a767d: Rename /tkmd-create to /tkmd-plan

## Description

Replace the user-facing `/tkmd-create` command and matching skill with
`/tkmd-plan`. Remove the old command name rather than keeping an alias, so the
plugin still exposes exactly four focused commands.

## Acceptance criteria

- [ ] The command palette exposes `/tkmd-plan` and no `/tkmd-create`.
- [ ] The matching skill is named `tkmd-plan` and command instructions invoke it.
- [ ] Plugin manifest, rules, documentation, examples, and tests use `/tkmd-plan`.
- [ ] The installed local Taskmark plugin is synchronized after the rename.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:38:00Z | prompt | Marco Mendão | Rename `/tkmd-create` to `/tkmd-plan` and make it organize user requirements into the optimal Taskmark hierarchy. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
