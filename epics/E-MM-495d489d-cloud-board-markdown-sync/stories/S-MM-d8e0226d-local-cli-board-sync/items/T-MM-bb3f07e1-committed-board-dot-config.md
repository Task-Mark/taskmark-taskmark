---
id: T-MM-bb3f07e1
type: task
title: Read committed board .config for cloud sync
status: done
priority: high
size: S
points: 3
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
tags: [cli, sync, config]
created: 2026-09-04
updated: 2026-09-04T09:17:33Z
started_at: 2026-09-04T09:14:00Z
completed_at: 2026-09-04T09:17:33Z
---
# T-MM-bb3f07e1: Read committed board .config for cloud sync

## Description

Keep the local Settings page as a per-machine sync token (stored under `~/.taskmark`, not in git). Also read a board-root `.config` file in dotenv form (`TASKMARK_SYNC_TOKEN`, optional `TASKMARK_CLOUD_URL`) that is committed so a clone of the board starts cloud sync as soon as `taskmark dev` or `taskmark serve` runs. Precedence: Settings, then `.config`, then environment / `.env`. Do not upload `.config` through board-sync file batches.

## Acceptance criteria

- [x] Local Settings still saves the token outside the repository and still starts sync.
- [x] A committed board `.config` with `TASKMARK_SYNC_TOKEN` is enough for a fresh clone to sync without opening Settings.
- [x] Settings overrides `.config` on that machine; `.config` overrides `TASKMARK_SYNC_TOKEN` in the environment.
- [x] Changing `.config` is picked up by the running watcher, same as Settings.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-04T09:14:00Z | prompt | Marco Mendão | Two ways to configure local cloud sync: existing Settings, plus a git-committed .config so clones start syncing immediately. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-04T09:14:00Z | 2026-09-04T09:17:33Z | Resolve sync credentials from Settings, then board `.config`, then env; watch `.config`; keep `.config` out of board-sync uploads. |
