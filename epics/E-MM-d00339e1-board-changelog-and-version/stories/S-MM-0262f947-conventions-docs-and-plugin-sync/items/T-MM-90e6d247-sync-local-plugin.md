---
id: T-MM-90e6d247
type: task
title: Sync local Taskmark plugin after command files land
status: backlog
priority: high
size: XS
points: 1
parent: S-MM-0262f947
epic: E-MM-d00339e1
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin]
created: 2026-08-29
updated: 2026-08-29T16:56:10Z
started_at: null
completed_at: null
---

# T-MM-90e6d247: Sync local Taskmark plugin after command files land

## Description

After the plugin package under `taskmark-cursor/plugins/taskmark` includes the new commands, skills, and convention/rule updates, rsync into `~/.cursor/plugins/local/taskmark` using the existing sync-plugin-local skill.

## Acceptance criteria

- [ ] Local plugin install contains `/tkmd-changelog` and `/tkmd-version` commands and skills
- [ ] Sync uses the existing rsync path; no extra derived board files

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T16:56:10Z | prompt | Marco Mendão | `/tkmd-save`: Cursor plan for `/tkmd-changelog` and `/tkmd-version` with CHANGELOG.md on the board and version on taskmark-taskmark package.json. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
