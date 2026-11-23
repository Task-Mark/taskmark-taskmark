---
id: S-MM-652cf8de
type: story
title: Dashboard aggregation API endpoint
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
tags: [api, dashboard, aggregation]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# S-MM-652cf8de: Dashboard aggregation API endpoint

## Description

New `dashboard` module in taskmark-api exposing `GET /dashboard` behind `JwtAuthGuard`. For every active membership of the user it loads the project `BoardState` and extracts a compact per-project payload from the stored snapshot (opaque `Mixed` JSON, defensive extraction with fallbacks): project identity and `lastSyncAt`, `statusMetrics`, flattened worklog rows (last 90 days, capped), enriched completion samples carrying resolvers for author filtering, active items (`in_progress` / `blocked`), presence cards, and `recentActivity`. Full snapshots (up to 8 MB each) never leave the API.

## User story

As a Cloud user with several projects, I want one API call that returns a small aggregated payload for all my projects so the dashboard loads fast without downloading every board snapshot.

## Acceptance criteria

- [ ] `GET /dashboard` returns one compact entry per active project membership, and nothing for projects the user is not an active member of.
- [ ] Each entry carries metrics, worklog rows (90-day window, per-project cap), completion samples with resolvers, active items, presence cards, and recent activity.
- [ ] Malformed or missing snapshot fields degrade to empty values instead of failing the request.
- [ ] The response size stays far below the full-snapshot cost regardless of board size.
