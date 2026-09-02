---
id: T-MM-0d6a60da
type: task
title: Push board files from TASKMARK_SYNC_TOKEN with watch
status: done
priority: high
size: L
points: 8
parent: S-MM-d8e0226d
epic: E-MM-495d489d
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
tags: [cli, sync]
created: 2026-09-02
updated: 2026-09-02T21:19:13Z
started_at: 2026-09-02T17:54:46Z
completed_at: 2026-09-02T18:07:57Z
---
# T-MM-0d6a60da: Push board files from TASKMARK_SYNC_TOKEN with watch

## Description

Add `npx taskmark sync [--watch]` that reads `TASKMARK_SYNC_TOKEN` and optional `TASKMARK_CLOUD_URL`, diffs hashes against the manifest, and pushes changed files plus a rebuilt snapshot. `taskmark dev` starts watch sync when the token is set; `serve` still uses `--sync`.

## Acceptance criteria

- [x] Sync prints the project name from the manifest and uploads only files whose hashes differ.
- [x] Watch mode debounces markdown changes and stops with a clear message on 401.
- [x] `taskmark dev` starts the watcher when `TASKMARK_SYNC_TOKEN` is set; `taskmark serve --sync` still starts it explicitly.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T21:19:13Z | prompt | Marco Mendão | `taskmark dev` should start sync watch automatically when TASKMARK_SYNC_TOKEN is set. |
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |
| 2026-09-02T17:54:46Z | prompt | Marco Mendão | From the Cursor plan Sync board local cloud: local CLI configured only by TASKMARK_SYNC_TOKEN, with optional watch alongside dev and serve. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T17:54:46Z | 2026-09-02T18:07:57Z | Added taskmark sync --watch from TASKMARK_SYNC_TOKEN. |
| Marco Mendão | 2026-09-02T21:19:13Z | 2026-09-02T21:19:13Z | Start cloud sync watch from taskmark dev when TASKMARK_SYNC_TOKEN is set. |
