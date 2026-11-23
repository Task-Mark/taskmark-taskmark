---
id: T-MM-0ff2e55d
type: task
title: Dashboard navigation link and periodic refresh
status: backlog
priority: high
size: S
points: 3
parent: S-MM-46b6e806
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, navigation, frontend]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-0ff2e55d: Dashboard navigation link and periodic refresh

## Description

Add a Dashboard link to `CloudBoardChrome` and `CloudMobileMenu` in `cloud-board-chrome.tsx`, with the path defined in `lib/project-routes.ts`. On the dashboard page, add a small client component that calls `router.refresh()` on a ~60-second interval so data stays current without opening one SSE connection per project.

## Acceptance criteria

- [ ] The Dashboard link appears in the desktop chrome and in the mobile hamburger menu on every Cloud page.
- [ ] The dashboard route path lives in `project-routes.ts` next to the other route helpers.
- [ ] Dashboard data refreshes roughly every 60 seconds while the page is open, with no per-project SSE connections.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — chrome/menu navigation link and 60s periodic refresh. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
