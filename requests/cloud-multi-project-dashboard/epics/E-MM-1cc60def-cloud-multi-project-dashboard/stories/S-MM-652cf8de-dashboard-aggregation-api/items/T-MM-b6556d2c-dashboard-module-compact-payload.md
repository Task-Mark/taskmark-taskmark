---
id: T-MM-b6556d2c
type: task
title: Dashboard module with GET /dashboard compact per-project payload
status: backlog
priority: high
size: L
points: 8
parent: S-MM-652cf8de
epic: E-MM-1cc60def
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [api, dashboard, nestjs]
created: 2026-09-15
updated: 2026-09-15T23:06:00Z
started_at: null
completed_at: null
---
# T-MM-b6556d2c: Dashboard module with GET /dashboard compact per-project payload

## Description

Create `taskmark-api/src/dashboard/` (module, controller, service) registered in `app.module.ts`. `GET /dashboard` uses `JwtAuthGuard`, finds the user's active memberships (same pattern as `requireMembership` in `boards.service.ts`), loads each project's `BoardState`, and extracts per project: `{ id, name, slug, role, lastSyncAt, version }`, the snapshot `statusMetrics` as-is, flattened worklog rows from `detailsByPath` (tasks/bugs only, mirroring `flattenWorklogEntries`, 90-day window, cap ~300 per project), enriched completion samples (`completedAt`, `points`, `resolvers`, `itemType`), active items with status `in_progress` or `blocked` (id, title, type, status, priority, points, assignees, epic, updated), plus the stored `presence` cards and `recentActivity`. Define minimal local DTO/types in the module — the API does not depend on `@taskmark/components`.

## Acceptance criteria

- [ ] `GET /dashboard` responds only for authenticated users and covers exactly their active project memberships.
- [ ] Per-project payload includes project identity, metrics, capped 90-day worklog rows, completion samples with resolvers, active items, presence cards, and recent activity.
- [ ] Projects with no snapshot yet appear with empty data and their `lastSyncAt: null` so the frontend can render setup hints.
- [ ] Snapshot extraction is defensive: unexpected shapes yield empty arrays/nulls, never a 500.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:06:00Z | prompt | Marco Mendão | Cursor plan: cloud multi-project dashboard — compact GET /dashboard aggregation endpoint on taskmark-api. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
