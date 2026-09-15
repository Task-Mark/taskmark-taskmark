---
id: S-MM-46b6e806
type: story
title: Dashboard page with global filters and navigation
status: backlog
priority: high
size: null
points: null
parent: E-MM-1cc60def
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [cloud, dashboard, frontend, filters]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# S-MM-46b6e806: Dashboard page with global filters and navigation

## Description

New `/dashboard` route in taskmark-cloud: a server component fetches `GET /dashboard` via `apiServer`, renders the existing `AppBar` with `CloudBoardChrome` / `CloudMobileMenu`, and hands the payload to a client wrapper that owns the global filter state (multi-select projects, multi-select authors, timeframe) applied to every widget. The dashboard is linked from the app bar and mobile menu and refreshes itself periodically.

## User story

As a Cloud user, I want a dashboard page I can reach from anywhere in the app, filter by project, author, and timeframe, and trust to stay current without reloading by hand.

## Acceptance criteria

- [ ] `/dashboard` renders for signed-in users with a loading state, and shows `EmptyProjectsHome` when the user has no projects.
- [ ] Project, author, and timeframe filters exist once at the top and every widget respects them.
- [ ] A Dashboard link is present in the desktop app bar chrome and in the mobile menu.
- [ ] The page refreshes its data roughly every 60 seconds without opening one SSE connection per project.
