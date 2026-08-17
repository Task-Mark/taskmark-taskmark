---
id: T-022
type: task
title: Initialize git for dedicated Taskmark project
status: done
priority: high
size: XS
size_source: suggested
size_basis: [T-019, T-002]
points: 1
points_source: suggested
estimate_minutes: 14
actual_minutes: 1
estimate_basis: [T-019]
session_cap_minutes: 480
parent: S-008
epic: E-003
owner: ""
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
tags: [git, multi-repo, init]
created: 2026-07-21
updated: 2026-08-17T08:03:41.619Z
started_at: 2026-07-21T22:20:51Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 60000
---

# T-022: Initialize git for dedicated Taskmark project

## Description

When creating the multi-project `<common>-taskmark` folder, run `git init` so the board has its own repository. Skip if `.git` already exists.

## Acceptance criteria

- [x] New dedicated Taskmark project has a `.git` directory after setup.
- [x] Existing git repos are left untouched (no re-init).
- [x] Board commits for multi-project work target this repo’s short name in Commits tables.

## Notes

Remote/push setup is out of scope for this task.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T22:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for Taskmark project structure refactor |
| 2 | 2026-07-21T22:36:37Z | feedback | Marco Mendão | E-003 delivered: hyphen -taskmark sibling board model |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T22:20:51Z | 2026-07-21T22:21:51Z | auto-backfilled: velocity × points (missing work log); shared-batch: 1 of 2min by points |
