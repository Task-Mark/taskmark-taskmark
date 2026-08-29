---
id: T-MO-1feb092b
type: task
title: Add /tkmd-shelf command, skill, and rules
status: done
priority: high
size: S
points: 3
parent: S-MO-71fe0e31
epic: E-MO-0b24529a
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
tags: [plugin, commands]
created: 2026-08-29
updated: 2026-08-29T11:06:17Z
started_at: 2026-08-29T10:58:00Z
completed_at: 2026-08-29T11:03:58Z
---

# T-MO-1feb092b: Add /tkmd-shelf command, skill, and rules

## Description

Add the user-facing `/tkmd-shelf` Cursor command and skill. Update always-apply project memory and plugin copy so shelf is a supported command with init, plan, do, and commit. Do not implement leaf markdown writes in this task.

## Acceptance criteria

- [x] `commands/tkmd-shelf.md` and `skills/tkmd-shelf/SKILL.md` exist and describe shelving a task, story, or epic without commit/push.
- [x] Always-apply rules list `/tkmd-shelf` with the other user commands.
- [x] Plugin description no longer claims exactly four commands.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T10:53:00Z | prompt | Marco Mendão | New `/tkmd-shelf` to discard never-implemented tasks/epics/stories; distinct from done; hide-completed hides shelved. |
| 2026-08-29T11:03:58Z | prompt | Marco Mendão | Implement E-MO-0b24529a and all open descendant leaves. |
| 2026-08-29T11:06:17Z | feedback | Marco Mendão | Apply necessary follow-up findings from the completed implementation audits. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T10:58:00Z | 2026-08-29T10:59:08Z | Added the shelf command, skill, project rule, and plugin copy. |
| Marco Mendão | 2026-08-29T11:05:00Z | 2026-08-29T11:05:14Z | Added plugin surface coverage and the markdown conventions rule. |
