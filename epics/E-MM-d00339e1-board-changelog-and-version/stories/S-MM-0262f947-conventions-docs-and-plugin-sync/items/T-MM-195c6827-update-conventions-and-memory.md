---
id: T-MM-195c6827
type: task
title: Update conventions and project-memory for changelog commands
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
tags: [conventions, plugin]
created: 2026-08-29
updated: 2026-08-29T16:56:10Z
started_at: null
completed_at: null
---

# T-MM-195c6827: Update conventions and project-memory for changelog commands

## Description

Extend the allowed `/tkmd-*` list with changelog and version. Replace “never write a changelog” with: do not generate changelog in the board README; `CHANGELOG.md` is written only by `/tkmd-changelog` and `/tkmd-version`. Those commands do not commit.

## Acceptance criteria

- [ ] `taskmark-conventions` skill and `.mdc` name `/tkmd-changelog` and `/tkmd-version` and their write boundaries
- [ ] `taskmark-project-memory.mdc` command list and changelog rule match
- [ ] Still forbids INDEX/SIZING/VELOCITY and generated board README dashboards

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
