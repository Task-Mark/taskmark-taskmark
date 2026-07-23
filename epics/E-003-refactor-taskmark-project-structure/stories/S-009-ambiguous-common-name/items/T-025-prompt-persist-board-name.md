---
id: T-025
type: task
title: Prompt user and persist board project name
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-024, T-004]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_basis: [calibrated:T-025]
session_cap_minutes: 480
parent: S-009
epic: E-003
owner: ""
blocked: false
cancelled: false
tags: [multi-repo, naming, ux]
created: 2026-07-21
updated: 2026-07-23T04:38:56.857Z
started_at: 2026-07-21T22:04:51Z
completed_at: 2026-07-21T22:36:51Z
actual_ms: 0
---
# T-025: Prompt user and persist board project name

## Description

When the common name is ambiguous, ask the user for the intended `<common_project_name>` (or full `<name>-taskmark` folder name), then persist the choice so later sessions reuse it.

## Acceptance criteria

- [x] Agent/skill prompts the user instead of guessing when T-024 flags ambiguity.
- [x] Choice is stored in board metadata (e.g. `REPOS.md` Canonical / Board project field).
- [x] Subsequent sync/init reads the persisted name and does not re-prompt unless missing.

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
| 1 | agent | 2026-07-21T22:04:51Z | 2026-07-21T22:04:51Z | auto-backfilled: velocity × points (missing work log); shared-batch: 0 of 1min by points |
