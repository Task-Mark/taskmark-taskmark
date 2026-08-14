---
id: T-277
type: task
title: Global taskmark workspace mode with project picker
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 6
estimate_source: suggested
estimate_basis: [calibrated:T-277]
session_cap_minutes: 480
parent: E-014
epic: E-014
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
tags: [frontend, cli, workspace, multi-project]
created: 2026-08-14
updated: 2026-08-14T17:50:46.835Z
started_at: 2026-08-14T17:32:36Z
completed_at: 2026-08-14T17:38:54Z
actual_ms: 378000
---
# T-277: Global taskmark workspace mode with project picker

## Description

Auto-binding (T-261, B-016) made every entry point single-board: `yarn dev` in `taskmark-frontend` binds to the sibling `taskmark-taskmark` board and hides the project selector, which is correct for local product development. But it also removed any way to run the UI across several boards, so a globally invoked `npx taskmark` can no longer pick which project's board to open.

Split the two entry points:

- `taskmark dev` / `taskmark serve` stay board-bound (auto-config from `--board`, env, cwd, or sibling `*-taskmark`) with no project selector.
- Bare `taskmark` (and `taskmark open`, or any command with `--workspace`) runs in workspace mode: auto-config binding is skipped, the setup wizard scans a master folder, and the app bar project selector plus "Add project" come back.

## Acceptance criteria

- [x] `yarn dev` in `taskmark-frontend` opens the sibling `taskmark-taskmark` board directly, with no project selector and no setup wizard.
- [x] Bare `npx taskmark` starts the prebuilt UI in workspace mode and lands on the setup wizard / project picker instead of a bound board.
- [x] Workspace mode ignores `TASKMARK_BOARD` / `TASKMARK_MASTER` / cwd binding so an inherited env cannot force a single board.
- [x] The setup wizard is pre-filled with the directory `taskmark` was invoked from so scanning for projects is one click.
- [x] `taskmark serve --workspace` and `taskmark dev --workspace` select workspace mode explicitly; `--board` together with `--workspace` is rejected.
- [x] Master folder discovery no longer skips directories named `taskmark`, so a workspace root with that name lists its boards.
- [x] CLI help and `README.md` document both modes.

## Notes

Workspace mode is signalled to the Next app with `TASKMARK_WORKSPACE=1`; the invocation directory travels as `TASKMARK_WORKSPACE_ROOT`. Multi-project state stays in the existing `taskmark_master_folders` / `taskmark_active_project` cookies.

`discoverTaskmarkProjects` skipped every child folder literally named `taskmark`, which hid `~/Projects/taskmark/*-taskmark` from the picker. A nested `<dir>/taskmark` board is already returned before that loop runs, so the skip only ever suppressed ordinary directories.

Verified with two dev servers: bound on :9101 redirected to `/board` with no `projectId` control; workspace on :9102 (launched from `~/Projects/taskmark`) redirected to `/setup` pre-filled with that path, and with master `~/Projects` saved it listed nine boards including `taskmark-taskmark`.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-08-14T17:32:36Z | prompt | Marco Mendão | yarn dev should open the local taskmark board directly; npx taskmark should run globally with a project picker |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-08-14T17:32:36Z | 2026-08-14T17:38:54Z | Added TASKMARK_WORKSPACE mode, `open` as the default CLI command, `--workspace` for serve/dev, setup pre-fill, and unskipped `taskmark`-named dirs in discovery |
