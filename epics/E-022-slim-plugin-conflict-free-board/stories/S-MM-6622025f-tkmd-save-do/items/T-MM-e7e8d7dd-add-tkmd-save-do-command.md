---
id: T-MM-e7e8d7dd
type: task
title: Add /tkmd-save-do command and skill
status: done
priority: high
size: M
points: 5
parent: S-MM-6622025f
epic: E-022
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
tags: [plugin, commands, planning, cursor-plan]
created: 2026-08-31
updated: 2026-08-31T12:29:40Z
started_at: 2026-08-31T12:23:49Z
completed_at: 2026-08-31T12:29:40Z
---

# T-MM-e7e8d7dd: Add /tkmd-save-do command and skill

## Description

Add a user-facing `/tkmd-save-do` slash command that composes the existing
`tkmd-save` and `tkmd-do` skills. After save finishes, if new item files were
created, implement that new work with `/tkmd-do` (the highest new parent when
a story or epic was created; otherwise each newly created leaf). Keep
`/tkmd-save` unchanged as a save-only command.

## Acceptance criteria

- [x] `commands/tkmd-save-do.md` and `skills/tkmd-save-do/SKILL.md` exist; the command tells the agent to use the `tkmd-save-do` skill.
- [x] The skill follows `tkmd-save` first (locate plan, search, dedupe, write new files only, carry visuals), then `tkmd-do` on newly created items only.
- [x] When save creates nothing, the skill reports the matching item and does not start implementation.
- [x] Safety matches `/tkmd-do`: no commit, no push, no `in_progress`; only executed leaf markdown may change during the do phase.
- [x] Plugin tests, `plugin.json`, always-apply rules, and plugin/repo READMEs allow this command; local plugin install is synced.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T12:23:49Z | prompt | Marco Mendão | `/tkmd-plan-do`: create `/tkmd-save-do`, similar to `/tkmd-save`, that saves a Cursor plan and then immediately executes the tasks that plan generated. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T12:23:49Z | 2026-08-31T12:27:28Z | Added `/tkmd-save-do` command, skill, plugin surface, tests, and synced the local plugin. |
