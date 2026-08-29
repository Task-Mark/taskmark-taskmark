---
id: T-MO-4e6a767d
type: task
title: Rename /tkmd-create to /tkmd-plan
status: done
priority: high
size: M
points: 5
parent: S-088
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
blocked: false
cancelled: false
tags: [plugin, commands, planning]
created: 2026-08-29
updated: 2026-08-29T10:48:48Z
started_at: 2026-08-29T10:42:00Z
completed_at: 2026-08-29T10:48:48Z
---

# T-MO-4e6a767d: Rename /tkmd-create to /tkmd-plan

## Description

Replace the user-facing `/tkmd-create` command and matching skill with
`/tkmd-plan`. Remove the old command name rather than keeping an alias, so the
plugin still exposes exactly four focused commands.

## Acceptance criteria

- [x] The command palette exposes `/tkmd-plan` and no `/tkmd-create`.
- [x] The matching skill is named `tkmd-plan` and command instructions invoke it.
- [x] Plugin manifest, rules, documentation, examples, and tests use `/tkmd-plan`.
- [x] The installed local Taskmark plugin is synchronized after the rename.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:38:00Z | prompt | Marco Mendão | Rename `/tkmd-create` to `/tkmd-plan` and make it organize user requirements into the optimal Taskmark hierarchy. |
| 2026-08-29T10:42:00Z | prompt | Marco Mendão | `/tkmd-do`: complete every remaining task in S-088. |
| 2026-08-29T10:48:48Z | feedback | Marco Mendão | Renamed command and skill, updated all current references and synchronized the local plugin. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T10:42:00Z | 2026-08-29T10:44:15Z | Renamed tkmd-create command and skill to tkmd-plan; updated plugin and website references. |
