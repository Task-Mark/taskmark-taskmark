---
id: T-027
type: task
title: Update sync-taskmark-repos skill and script
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-023, T-026]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 1
estimate_basis: [calibrated:T-027]
session_cap_minutes: 480
parent: S-010
epic: E-003
owner: ""
blocked: false
cancelled: false
tags: [plugin, sync, multi-repo]
created: 2026-07-21
updated: 2026-07-23T15:41:41.235Z
started_at: 2026-07-21T21:48:51Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 60000
---

# T-027: Update sync-taskmark-repos skill and script

## Description

Rewrite `sync-taskmark-repos` skill and `scripts/sync-taskmark-repos.sh` for the new model: ensure dedicated board project exists in multi mode; do not rsync `taskmark/` into product repos; keep `REPOS.md` product-root listing accurate.

## Acceptance criteria

- [x] Skill steps match dedicated-board semantics.
- [x] Script no longer copies the board tree into every discovered git root.
- [x] Multi mode resolves/creates the `-taskmark` project as canonical.
- [x] Single mode is a no-op copy (board already in project).

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T22:26:00Z | prompt | Create epic + stories/tasks for Taskmark project structure refactor |
| 2 | 2026-07-21T22:36:37Z | feedback | E-003 delivered: hyphen -taskmark sibling board model |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T21:48:51Z | 2026-07-21T21:49:51Z | auto-backfilled: velocity × points (missing work log); shared-batch: 1 of 3min by points |
