---
id: T-MM-e8c53f7d
type: task
title: Verify deletes leftover generated board files
status: done
priority: high
size: S
points: 3
parent: S-MM-ac500104
epic: E-022
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
tags: [plugin, migration, board]
created: 2026-08-31
updated: 2026-08-31T13:06:14Z
started_at: 2026-08-31T13:01:00Z
completed_at: 2026-08-31T13:06:14Z
---

# T-MM-e8c53f7d: Verify deletes leftover generated board files

At the canonical board root only, delete `INDEX.md`, `SIZING.md`, `VELOCITY.md`, and shared ID counter files (`NEXT_IDS` / `NEXT_IDS.md` and similar) when present. After the static README is in the correct place, delete a nested `taskmark/README.md` that is still a generated dashboard. Do not delete an existing `CHANGELOG.md`, `epics/`, `node_modules/`, or `out/`.

## Acceptance criteria

- [x] `INDEX.md`, `SIZING.md`, and `VELOCITY.md` at the board root are removed when they exist.
- [x] Shared ID counter files at the board root are removed when they exist.
- [x] A nested generated dashboard README is removed only after the static project README lives in the init location.
- [x] Existing `CHANGELOG.md` and `epics/` are left in place.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T12:22:27Z | prompt | Marco Mendão | Cursor plan: `/tkmd-verify` migrates old boards to the current Taskmark layout and item spec. |
| 2026-08-31T13:01:00Z | prompt | Marco Mendão | `/tkmd-do S-MM-ac500104`: implement `/tkmd-verify` to migrate old boards. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T13:01:00Z | 2026-08-31T13:01:41Z | `verify-board.py` deletes leftover generated files and keeps CHANGELOG and epics. |
