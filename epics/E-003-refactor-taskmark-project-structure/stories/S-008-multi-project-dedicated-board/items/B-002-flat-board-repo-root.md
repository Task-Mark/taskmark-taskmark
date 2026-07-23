---
id: B-002
type: bug
title: Dedicated board repo must be flat (no nested taskmark/)
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-021, T-023]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 32
estimate_basis: [calibrated:B-002]
session_cap_minutes: 480
parent: S-008
epic: E-003
owner: ""
blocked: false
cancelled: false
tags: [architecture, multi-repo, layout]
created: 2026-07-21
updated: 2026-07-23T09:47:44.562Z
started_at: 2026-07-21T22:40:35Z
completed_at: 2026-07-21T22:40:35Z
actual_ms: 1920000
---

# B-002: Dedicated board repo must be flat (no nested taskmark/)

## Description

In multi-project mode, `<common>-taskmark` nested the board under `taskmark/` (`<name>-taskmark/taskmark/`). The dedicated project root should **be** the board.

## Repro steps

1. Multi-git workspace sync creates or uses `<common>-taskmark`.
2. Observe `INDEX.md` under `<common>-taskmark/taskmark/` instead of at the repo root.

## Fix criteria

- [x] Multi-project board files live at `<common>-taskmark/` root (`INDEX.md`, `epics/`, `REPOS.md`).
- [x] Sync script flattens legacy nested `taskmark/` folders.
- [x] Docs, init, and always-apply rule forbid `<name>-taskmark/taskmark/`.
- [x] This workspace migrated to the flat layout.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T22:40:35Z | prompt | Multi-project: root <name>-taskmark should be the board; avoid nested taskmark/ |
| 2 | 2026-07-21T22:40:35Z | feedback | Flattened board; updated sync script and conventions |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|
| 9510b02 | taskmark-taskmark | 2026-07-21T22:42:00Z | add flat taskmark board |
| f742175 | taskmark-cursor | 2026-07-21T22:42:00Z | flatten multi-repo board layout |
| 4605512 | taskmark-frontend | 2026-07-21T22:42:00Z | remove nested taskmark board copy |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T22:08:35Z | 2026-07-21T22:40:35Z | auto-backfilled: velocity × points (missing work log) |
