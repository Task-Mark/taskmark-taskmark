---
id: T-MM-a89041bf
type: task
title: Cover /tkmd-reportme in the tests and sync the local plugin
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
tags: [tests, plugin, reports]
created: 2026-08-31
updated: 2026-08-31T06:47:12Z
started_at: null
completed_at: null
---

# T-MM-a89041bf: Cover /tkmd-reportme in the tests and sync the local plugin

## Description

The plugin test suite asserts the exact command and skill sets, so both need the new entry or the suite fails. Add a check that the report skill states the identity filter, the `.reports/report-` write target, and the no-commit boundary, and extend the init helper test so a report path is confirmed gitignored. Then sync the plugin package into the local install so the command is available in Cursor.

## Acceptance criteria

- [ ] The expected command set and skill set include the report command
- [ ] A test asserts the identity filter, the report write target, and the no-commit boundary
- [ ] The init helper test confirms a report path is gitignored on a fresh board
- [ ] The full plugin test suite passes
- [ ] The local plugin install is synced from the package

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T06:47:12Z | prompt | Marco Mendão | From a Cursor plan: the new report command must be guarded by the plugin test suite and available in the local install. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
