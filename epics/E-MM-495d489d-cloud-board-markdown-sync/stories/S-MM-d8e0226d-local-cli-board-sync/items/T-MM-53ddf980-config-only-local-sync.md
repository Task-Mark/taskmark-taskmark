---
id: T-MM-53ddf980
type: task
title: Read local sync settings only from board .config
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
tags: [local-ui, settings, sync, config]
created: 2026-09-15
updated: 2026-09-15T12:27:30Z
started_at: 2026-09-15T12:22:00Z
completed_at: 2026-09-15T12:27:30Z
---
# T-MM-53ddf980: Read local sync settings only from board .config

## Description

Remove the Settings tab from bound local Taskmark boards. Cloud sync credentials for a local project come only from the committed board-root `.config` file (`TASKMARK_SYNC_TOKEN`, optional `TASKMARK_CLOUD_URL`), not from a per-machine Settings page or `~/.taskmark` override. Environment variables remain a fallback when `.config` has no valid token.

## User story

As a developer, I configure local cloud sync by editing the board `.config` file so the local UI has no Settings tab and every clone uses the same committed credentials.

## Acceptance criteria

- [x] Bound local boards do not show a Settings tab or page for saving a sync token.
- [x] `taskmark dev` / `taskmark serve` / `taskmark sync` resolve credentials from board `.config`, then environment / `.env`.
- [x] A token stored under `~/.taskmark` no longer overrides `.config`.
- [x] Cloud setup copy tells people to put the token in the local board `.config` file.
- [x] Config resolution tests pass.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T12:22:00Z | prompt | Marco Mendão | Remove the Settings tab from local projects; all settings should be read from the `.config` file. |
| 2026-09-15T12:36:30Z | feedback | Marco Mendão | Checked that board markdown edits still reach Taskmark Cloud after the Settings removal. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T12:22:00Z | 2026-09-15T12:27:30Z | Removed local Settings UI and ~/.taskmark override; local sync now reads board `.config` (then env). |
