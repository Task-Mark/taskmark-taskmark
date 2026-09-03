---
id: T-MM-73171ed1
type: task
title: Start sync automatically from the saved project token
status: done
priority: high
size: M
points: 5
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
tags: [cli, sync, watch]
created: 2026-09-03
updated: 2026-09-03T15:15:39Z
started_at: 2026-09-03T15:04:18Z
completed_at: 2026-09-03T15:15:39Z
---
# T-MM-73171ed1: Start sync automatically from the saved project token

## Description

Make bound `taskmark dev` and `taskmark serve` watch the per-board sync configuration as well as markdown. Saving or replacing a token from Settings starts or retries synchronization without restarting Taskmark.

## Acceptance criteria

- [x] Bound `taskmark dev` and `taskmark serve` always monitor local sync configuration without requiring `--sync`.
- [x] Saving a token starts an initial sync automatically and subsequent markdown changes continue syncing.
- [x] Replacing an invalid token retries sync without restarting the local process.
- [x] Explicit `taskmark sync` still works and environment variables remain a fallback.
- [x] Watcher and CLI checks pass.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T15:04:18Z | prompt | Marco Mendão | Start synchronization automatically as soon as the cloud-generated token is saved in local project Settings. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-03T15:04:18Z | 2026-09-03T15:15:39Z | Made bound dev and serve watch per-board sync settings, recover after missing or rejected tokens, and start sync immediately after Settings saves. |
