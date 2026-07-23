---
id: T-020
type: task
title: Derive common project name
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-008, T-017]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 1
estimate_basis: [calibrated:T-020]
session_cap_minutes: 480
parent: S-008
epic: E-003
owner: ""
blocked: false
cancelled: false
tags: [architecture, multi-repo, naming]
created: 2026-07-21
updated: 2026-07-23T15:41:41.235Z
started_at: 2026-07-21T22:04:51Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 60000
---

# T-020: Derive common project name

## Description

From multiple workspace git roots, derive a confident `<common_project_name>` (e.g. shared parent folder name or shared prefix like `taskmark` from `taskmark-frontend` / `taskmark-cursor`) used to name `<common>-taskmark`.

## Acceptance criteria

- [x] Documented heuristic for common name (parent dir, shared prefix, etc.).
- [x] Returns a name when confidence is high.
- [x] Defers to S-009 / T-024 when confidence is low.

## Notes

Example for this workspace: parent `taskmark` → `taskmark-taskmark` may be wrong; prefer shared prefix `taskmark` → `taskmark-taskmark` is awkward — heuristics should prefer parent folder or ask (S-009). Capture preferred rule in implementation.

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
| 1 | agent | 2026-07-21T22:04:51Z | 2026-07-21T22:05:51Z | auto-backfilled: velocity × points (missing work log); shared-batch: 1 of 2min by points |
