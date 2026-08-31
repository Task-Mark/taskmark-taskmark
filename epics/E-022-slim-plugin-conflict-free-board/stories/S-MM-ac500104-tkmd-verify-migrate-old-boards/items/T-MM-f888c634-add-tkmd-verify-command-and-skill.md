---
id: T-MM-f888c634
type: task
title: Add /tkmd-verify command, skill, and allowlists
status: done
priority: high
size: M
points: 5
parent: S-MM-ac500104
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
tags: [plugin, commands, migration]
created: 2026-08-31
updated: 2026-08-31T13:06:14Z
started_at: 2026-08-31T13:01:00Z
completed_at: 2026-08-31T13:06:14Z
---

# T-MM-f888c634: Add /tkmd-verify command, skill, and allowlists

Add `commands/tkmd-verify.md` and `skills/tkmd-verify/SKILL.md` in the same shape as `/tkmd-reportme`. The skill states non-negotiable safety (no commit, no push, no creating INDEX/SIZING/VELOCITY/CHANGELOG) and the four phases: locate board, repair scaffold, delete forbidden generated files, migrate item markdown, then report. List the command in conventions, the always-apply project-memory rule, plugin and repo READMEs, plugin marketplace descriptions, and `test_plugin.py`. Sync the local plugin install.

## Acceptance criteria

- [x] `commands/tkmd-verify.md` tells the agent to use the `tkmd-verify` skill.
- [x] The skill exists, reads conventions first, and forbids commit, push, and creating `INDEX.md`, `SIZING.md`, `VELOCITY.md`, or `CHANGELOG.md`.
- [x] Conventions, project-memory allowlist, plugin/repo READMEs, and plugin descriptions include `/tkmd-verify`.
- [x] Plugin tests expect the new command and skill; the local plugin install is synced.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T12:22:27Z | prompt | Marco Mendão | Cursor plan: `/tkmd-verify` migrates old boards to the current Taskmark layout and item spec. |
| 2026-08-31T13:01:00Z | prompt | Marco Mendão | `/tkmd-do S-MM-ac500104`: implement `/tkmd-verify` to migrate old boards. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T13:01:00Z | 2026-08-31T13:02:08Z | Added `/tkmd-verify` command, skill, allowlists, and synced the local plugin. |
