---
id: T-028
type: task
title: Update init and related skills
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-027, T-026]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 5
estimate_basis: [calibrated:T-028]
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
tags: [plugin, init, skills]
created: 2026-07-21
updated: 2026-07-29T11:30:07.936Z
started_at: 2026-07-21T21:48:51Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 300000
---
# T-028: Update init and related skills

## Description

Update `taskmark-init`, create/start/complete/log-commits/commit-all, and any skill that assumes per-repo board copies so they locate the board in the project (single) or dedicated `-taskmark` repo (multi).

## Acceptance criteria

- [x] Init chooses correct target path by workspace mode.
- [x] Skills that previously called “sync copies to all repos” point at the new sync behavior.
- [x] Local plugin package synced after edits (`sync-plugin-local`).

## Notes

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
| 1 | Marco Mendão | 2026-07-21T21:48:51Z | 2026-07-21T21:53:51Z | auto-backfilled: velocity × points (missing work log); shared-batch: 5 of 9min by points |
