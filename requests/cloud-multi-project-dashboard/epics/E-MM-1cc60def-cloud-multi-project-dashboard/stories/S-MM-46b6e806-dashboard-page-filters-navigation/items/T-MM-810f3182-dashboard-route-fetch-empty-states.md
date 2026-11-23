---
id: T-MM-810f3182
type: task
title: Dashboard route with server fetch and empty states
status: backlog
priority: high
size: M
points: 5
parent: S-MM-46b6e806
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, nextjs, dashboard]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-810f3182: Dashboard route with server fetch and empty states

## Description

Add `taskmark-cloud/app/dashboard/page.tsx` (server component) and `loading.tsx`. Fetch `GET /dashboard` with `apiServer`, add `DashboardResponse` types to `lib/api.ts`, and render the `AppBar` with the existing `CloudBoardChrome` / `CloudMobileMenu`. Handle empty states: no projects at all shows `EmptyProjectsHome`; projects that never synced render a card pointing at the sync setup instructions on that project's settings page.

## Acceptance criteria

- [ ] `/dashboard` server-renders from one `GET /dashboard` call with a skeleton `loading.tsx`.
- [ ] A user without projects sees `EmptyProjectsHome`; an API failure shows a readable error state.
- [ ] Never-synced projects are visible with a link to their settings setup instructions instead of empty widgets.
- [ ] Payload types live in `lib/api.ts` alongside the existing API types.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — /dashboard route, server fetch, and empty states. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
