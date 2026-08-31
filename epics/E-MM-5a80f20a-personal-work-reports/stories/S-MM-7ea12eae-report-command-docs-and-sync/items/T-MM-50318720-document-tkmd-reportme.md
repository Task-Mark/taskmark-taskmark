---
id: T-MM-50318720
type: task
title: Document /tkmd-reportme in rules, READMEs, and plugin metadata
status: backlog
priority: medium
size: S
points: 3
parent: S-MM-7ea12eae
epic: E-MM-5a80f20a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [docs, plugin, reports]
created: 2026-08-31
updated: 2026-08-31T06:47:12Z
started_at: null
completed_at: null
---

# T-MM-50318720: Document /tkmd-reportme in rules, READMEs, and plugin metadata

## Description

Add the command to every place the Taskmark command set is declared: the allowlist in the always-applied project-memory rule, with a line stating it writes only gitignored files under the board `.reports/` directory; the write-boundary list in the conventions skill; the plugin README bullet list; and the repository README command table. Refresh the plugin and marketplace descriptions, which currently omit the changelog and version commands as well.

## Acceptance criteria

- [ ] The project-memory rule lists `/tkmd-reportme` in the allowlist with its write boundary
- [ ] The conventions skill records that the command never implements, commits, or pushes and writes only report files
- [ ] The plugin README and repository README both list the command
- [ ] Plugin and marketplace descriptions name the full current command set

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T06:47:12Z | prompt | Marco Mendão | From a Cursor plan: a new `/tkmd-reportme` command needs to be part of the documented, allowed Taskmark command set. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
