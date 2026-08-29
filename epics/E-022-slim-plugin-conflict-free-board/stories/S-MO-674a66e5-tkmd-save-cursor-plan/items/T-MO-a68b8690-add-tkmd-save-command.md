---
id: T-MO-a68b8690
type: task
title: Add /tkmd-save command and skill
status: done
priority: high
size: M
points: 5
parent: S-MO-674a66e5
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [plugin, commands, planning, cursor-plan]
created: 2026-08-29
updated: 2026-08-29T11:14:10Z
started_at: 2026-08-29T11:09:00Z
completed_at: 2026-08-29T11:14:10Z
---

# T-MO-a68b8690: Add /tkmd-save command and skill

## Description

Add a user-facing `/tkmd-save` slash command and `tkmd-save` skill. After the
user finishes Cursor Plan mode, the skill locates that plan artifact, searches
the canonical board for overlaps, and creates the smallest useful epic / story /
task / bug hierarchy from the plan—same write boundaries as `/tkmd-plan` (new
item files only; no parent rewrites; no derived board files). Do not implement
work; that remains `/tkmd-do` or `/tkmd-plan-do`.

## Acceptance criteria

- [x] `commands/tkmd-save.md` and `skills/tkmd-save/SKILL.md` exist; the command tells the agent to use the `tkmd-save` skill.
- [x] The skill reads the Cursor Plan mode plan for the session (or an explicit plan path/target the user supplies) and maps sections into Taskmark types using conventions + `tkmd-plan` hierarchy rules.
- [x] Before writing, it searches open and done board items and creates nothing when an exact or overlapping item already covers the plan; it reports the match instead.
- [x] New files use `allocate-id.py`, correct `parent`/`epic` frontmatter, leaf Prompt & feedback on tasks/bugs only, and never edit pre-existing parents or derived markdown.
- [x] Plugin surface (`plugin.json`, always-apply rules, plugin/repo READMEs) lists `/tkmd-save`; local plugin install is synced. No commit, push, or `in_progress`.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:58:33Z | prompt | Marco Mendão | Add `/tkmd-save` after Cursor Plan mode: split the plan into epic/story/task/bug work items and keep plan diagrams/visuals on those items. |
| 2026-08-29T11:09:00Z | prompt | Marco Mendão | `/tkmd-do`: implement every backlog work item under epic E-022. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:09:00Z | 2026-08-29T11:10:14Z | Added `/tkmd-save` command, skill, plugin surface, tests, and local sync. |
