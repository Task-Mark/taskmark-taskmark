---
id: T-MM-6e3393d4
type: task
title: Stale sync alert banner
status: backlog
priority: medium
size: S
points: 3
parent: S-MM-ce20fdf4
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, frontend, sync]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-6e3393d4: Stale sync alert banner

## Description

Banner at the top of the dashboard listing projects whose `lastSyncAt` is older than 7 days or that never synced, each with a direct link to that project's settings page where the sync token setup instructions live. The banner complements the stale flag on the project health cards and hides when everything is fresh.

## Acceptance criteria

- [ ] The banner lists every project not synced in the last 7 days, including never-synced projects.
- [ ] Each entry links to that project's settings/setup instructions.
- [ ] With no stale projects the banner does not render.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — top banner alerting on projects without recent sync. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
