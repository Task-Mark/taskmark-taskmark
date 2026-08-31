---
id: T-MM-c779921b
type: task
title: Keep generated reports out of git and images
status: backlog
priority: high
size: S
points: 3
parent: S-MM-6b6bcec6
epic: E-MM-5a80f20a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, gitignore, reports]
created: 2026-08-31
updated: 2026-08-31T06:47:12Z
started_at: null
completed_at: null
---

# T-MM-c779921b: Keep generated reports out of git and images

## Description

Reports are personal and local, so `.reports/` must be ignored everywhere `REPOS.md` already is. Add the entry to the ignore list written by `ensure-board-ui.py`, to the existing board `.gitignore` (which the script only merges into on a fresh run), and to the board-UI stub `.dockerignore` plus the board's own copy so hosted static images never carry local reports. Note in the commit skill that report files must not be staged.

## Acceptance criteria

- [ ] `ensure-board-ui.py` writes `.reports/` into a new or existing board `.gitignore`
- [ ] The current board `.gitignore` lists `.reports/`
- [ ] `git check-ignore` confirms a report path is ignored on a freshly initialised board
- [ ] The stub and board `.dockerignore` exclude `.reports/`
- [ ] The commit skill states that report files are gitignored and must not be staged

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T06:47:12Z | prompt | Marco Mendão | From a Cursor plan: report files must be ignored by git and live in a `.reports` folder rather than at the board root. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
