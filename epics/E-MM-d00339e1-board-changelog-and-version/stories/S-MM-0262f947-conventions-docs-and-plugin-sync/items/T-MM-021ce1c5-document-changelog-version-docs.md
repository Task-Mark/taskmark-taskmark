---
id: T-MM-021ce1c5
type: task
title: Document changelog and version commands in docs and READMEs
status: backlog
priority: high
size: S
points: 3
parent: S-MM-0262f947
epic: E-MM-d00339e1
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [docs, readme]
created: 2026-08-29
updated: 2026-08-29T16:56:10Z
started_at: null
completed_at: null
---

# T-MM-021ce1c5: Document changelog and version commands in docs and READMEs

## Description

Add `/tkmd-changelog` and `/tkmd-version` to the plugin README, board-root README command table, website docs nav, and `/docs/commands` (and setup/workflows/overview if they list every slash). `/tkmd-commit` stays the only commit command.

## Acceptance criteria

- [ ] Plugin README lists both commands with the Unreleased → version flow
- [ ] Board README command table includes both commands
- [ ] Website commands page and `DOCS_COMMANDS` include both; other docs that enumerate slashes stay consistent
- [ ] Copy does not revive a generated README changelog

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
