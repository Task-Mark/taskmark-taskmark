---
id: T-MM-60065930
type: task
title: Configure cloud sync from local project Settings
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
tags: [local-ui, settings, sync, security]
created: 2026-09-03
updated: 2026-09-03T18:09:00Z
started_at: 2026-09-03T15:04:18Z
completed_at: 2026-09-03T15:15:39Z
---
# T-MM-60065930: Configure cloud sync from local project Settings

## Description

Add a Settings page to each locally bound Taskmark project where a developer can paste the cloud-generated sync token. Store the secret in user-local Taskmark configuration outside the project repository and show only a safe hint after saving.

## Acceptance criteria

- [x] A bound local board exposes a Settings link and page for cloud synchronization.
- [x] The page accepts a valid `tmk_` token, reports errors, and never returns the stored token to the browser.
- [x] The token is stored per canonical board path under user-local Taskmark configuration with restrictive file permissions, outside the project repository.
- [x] Existing environment-variable configuration remains a backward-compatible fallback.
- [x] Config storage and UI checks pass.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T15:04:18Z | prompt | Marco Mendão | Replace manual sync-token environment variables with a per-project local Settings page where the cloud-generated token can be configured. |
| 2026-09-03T18:09:00Z | prompt | Marco Mendão | Add verbose step-by-step instructions on local Settings to configure Taskmark Cloud, pointing at cloud.taskmark.dev. |
| 2026-09-03T18:09:00Z | feedback | Marco Mendão | Official Cloud URL is cloud.taskmark.dev; copy should be more verbose so users know what to do. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-03T15:04:18Z | 2026-09-03T15:15:39Z | Added bound-board sync Settings, secure per-board user-local token storage, masked status, same-origin writes, and cloud setup guidance. |
| Marco Mendão | 2026-09-03T18:09:00Z | 2026-09-03T18:09:00Z | Added numbered local Settings steps for connecting a board to Taskmark Cloud. |
