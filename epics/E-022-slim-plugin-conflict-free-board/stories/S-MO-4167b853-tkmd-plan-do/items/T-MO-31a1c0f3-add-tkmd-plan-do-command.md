---
id: T-MO-31a1c0f3
type: task
title: Add /tkmd-plan-do command and skill
status: backlog
priority: high
size: M
points: 5
parent: S-MO-4167b853
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
updated: 2026-08-29T10:55:00Z
started_at: null
completed_at: null
---

# T-MO-31a1c0f3: Add /tkmd-plan-do command and skill

## Description

Add a user-facing `/tkmd-plan-do` slash command that composes the existing
`tkmd-plan` and `tkmd-do` skills. After planning finishes, if new item files
were created, implement that new work with `/tkmd-do` (the highest new parent
when a story or epic was created; otherwise each newly created leaf). Keep
`/tkmd-plan` unchanged as a plan-only command.

## Acceptance criteria

- [ ] `commands/tkmd-plan-do.md` and `skills/tkmd-plan-do/SKILL.md` exist; the command tells the agent to use the `tkmd-plan-do` skill.
- [ ] The skill follows `tkmd-plan` first (search, dedupe, write new files only), then `tkmd-do` on newly created items only.
- [ ] When planning creates nothing, the skill reports the matching item and does not start implementation.
- [ ] Safety matches `/tkmd-do`: no commit, no push, no `in_progress`; only executed leaf markdown may change during the do phase.
- [ ] Plugin tests, `plugin.json`, always-apply rules, and plugin/repo READMEs allow this fifth command; local plugin install is synced.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:55:00Z | prompt | Marco Mendão | Add `/tkmd-plan-do`: same as `/tkmd-plan`, then run `/tkmd-do` on the tasks just created. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
