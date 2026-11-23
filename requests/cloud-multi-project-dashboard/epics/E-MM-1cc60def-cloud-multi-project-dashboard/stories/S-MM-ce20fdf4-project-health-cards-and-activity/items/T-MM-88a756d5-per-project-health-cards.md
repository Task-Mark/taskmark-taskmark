---
id: T-MM-88a756d5
type: task
title: Per-project health cards
status: backlog
priority: high
size: M
points: 5
parent: S-MM-ce20fdf4
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, frontend, projects]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-88a756d5: Per-project health cards

## Description

One card per project: name, last sync time with a visual stale flag when `lastSyncAt` is older than 7 days, done/total progress with `ChildProgressBar`, average velocity formatted with `formatSpeedPtsPerWeek` (current vs peak from `statusMetrics`), contributor avatars via `ProjectContributorsPanel`-style avatars, and a link to the project board.

## Acceptance criteria

- [ ] Every selected project shows a card with progress, velocity (current and peak), contributors, and last sync.
- [ ] Cards for projects not synced in over 7 days, or never synced, carry a clear stale indicator.
- [ ] Each card links to its project board page.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — project health cards with velocity, progress, contributors, and sync state. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
