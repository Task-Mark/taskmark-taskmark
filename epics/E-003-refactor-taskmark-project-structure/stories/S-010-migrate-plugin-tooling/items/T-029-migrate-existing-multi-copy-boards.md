---
id: T-029
type: task
title: Migrate existing multi-copy boards
status: done
priority: medium
size: M
size_source: suggested
size_basis: [T-023, T-027]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_basis: [calibrated:T-029]
session_cap_minutes: 480
parent: S-010
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
tags: [migration, multi-repo, plugin]
created: 2026-07-21
updated: 2026-07-28T06:20:01.202Z
started_at: 2026-07-21T21:48:51Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 0
---
# T-029: Migrate existing multi-copy boards

## Description

Document and implement a migration path for workspaces that already keep identical `taskmark/` copies in every product repo: promote one canonical tree into `<name>-taskmark`, init git, update `REPOS.md`, and remove or stop syncing leftover copies.

## Acceptance criteria

- [x] Migration steps are documented for agents and humans.
- [x] Script or skill path can promote the richest/canonical copy into the dedicated project.
- [x] Guidance covers conflict resolution when copies diverged.
- [x] After migration, product repos no longer receive board copies.

## Notes

This workspace (taskmark-frontend + taskmark-cursor) is a target example.

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
| 1 | Marco Mendão | 2026-07-21T21:48:51Z | 2026-07-21T21:48:51Z | auto-backfilled: velocity × points (missing work log); shared-batch: 0 of 2min by points |
