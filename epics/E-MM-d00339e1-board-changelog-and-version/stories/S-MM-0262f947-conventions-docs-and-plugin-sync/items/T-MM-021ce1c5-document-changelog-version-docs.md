---
id: T-MM-021ce1c5
type: task
title: Document changelog and version commands in docs and READMEs
status: done
priority: high
size: S
points: 3
parent: S-MM-0262f947
epic: E-MM-d00339e1
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
tags: [docs, readme]
created: 2026-08-29
updated: 2026-08-29T17:18:08Z
started_at: 2026-08-29T17:13:00Z
completed_at: 2026-08-29T17:18:08Z
---

# T-MM-021ce1c5: Document changelog and version commands in docs and READMEs

## Description

Add `/tkmd-changelog` and `/tkmd-version` to the plugin README, board-root README command table, website docs nav, and `/docs/commands` (and setup/workflows/overview if they list every slash). `/tkmd-commit` stays the only commit command.

## Acceptance criteria

- [x] Plugin README lists both commands with the Unreleased → version flow
- [x] Board README command table includes both commands
- [x] Website commands page and `DOCS_COMMANDS` include both; other docs that enumerate slashes stay consistent
- [x] Copy does not revive a generated README changelog

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T16:56:10Z | prompt | Marco Mendão | `/tkmd-save`: Cursor plan for `/tkmd-changelog` and `/tkmd-version` with CHANGELOG.md on the board and version on taskmark-taskmark package.json. |
| 2026-08-29T17:13:00Z | prompt | Marco Mendão | `/tkmd-do`: implement every open descendant of epic E-MM-d00339e1. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T17:13:00Z | 2026-08-29T17:13:44Z | Documented changelog and version commands in READMEs and docs. |
