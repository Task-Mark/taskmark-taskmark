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
updated: 2026-09-03T09:03:39Z
started_at: 2026-09-02T17:54:46Z
completed_at: 2026-09-02T18:07:57Z
---
# T-MM-0d6a60da: Push board files from TASKMARK_SYNC_TOKEN with watch

## Description

Add `npx taskmark sync [--watch]` that reads `TASKMARK_SYNC_TOKEN` and optional `TASKMARK_CLOUD_URL`, diffs hashes against the manifest, and pushes changed files plus a rebuilt snapshot. `taskmark dev` starts watch sync when the token is set; `serve` still uses `--sync`. Without `TASKMARK_CLOUD_URL` the CLI targets the hosted `https://cloud.taskmark.dev`; local and self-hosted configurations point to their Taskmark Cloud origin, which proxies `/v1` to the backend API.

## Acceptance criteria

- [x] Sync prints the project name from the manifest and uploads only files whose hashes differ.
- [x] Watch mode debounces markdown changes and stops with a clear message on 401.
- [x] `taskmark dev` starts the watcher when `TASKMARK_SYNC_TOKEN` is set; `taskmark serve --sync` still starts it explicitly.
- [x] With no `TASKMARK_CLOUD_URL`, sync targets `https://cloud.taskmark.dev`; the cloud app answers `/v1` and forwards bearer tokens to the API.
- [x] A connection failure names the URL that was tried instead of a bare `fetch failed`.
- [x] The snapshot builder runs from an installed package under node_modules, where `@/` aliases and the TypeScript-only `@taskmark/components` break every TS runner.
- [x] `TASKMARK_CLOUD_URL` names the cloud app, which proxies to the API; the CLI never targets the API directly.
- [x] Every sync step prints progress: target cloud, project, file counts, snapshot build, each upload batch, and the resulting board version.
- [x] Uploads split into batches under the API's 400-file cap, with the snapshot attached to the final batch.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T09:03:39Z | prompt | Marco Mendão | Sync still is not happening: print sync logs in the console, and target the taskmark-cloud proxy instead of the API directly. |
| 2026-09-03T08:45:22Z | feedback | Marco Mendão | Sync now reaches the cloud but the snapshot build fails with ERR_MODULE_NOT_FOUND on `@/lib`. |
| 2026-09-02T21:31:52Z | prompt | Marco Mendão | Default to cloud.taskmark.dev when TASKMARK_CLOUD_URL is not provided. |
| 2026-09-02T21:24:00Z | feedback | Marco Mendão | Ran dev with the token but nothing synced: the client defaulted to localhost:4000 while the API listens on 8002. |
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
| Marco Mendão | 2026-09-02T21:24:00Z | 2026-09-02T21:31:52Z | Default sync to cloud.taskmark.dev, serve /v1 from the cloud app with bearer forwarding, and name the URL in connection errors. |
| Marco Mendão | 2026-09-03T08:38:00Z | 2026-09-03T08:45:22Z | Build the sync snapshot with esbuild instead of tsx, bundling @taskmark/components and sharing the externals rule with the static build. |
| Marco Mendão | 2026-09-03T08:51:00Z | 2026-09-03T09:03:39Z | Log every sync step, batch uploads under the API cap, keep watching after a failed first sync, and point the board at the cloud proxy. |
