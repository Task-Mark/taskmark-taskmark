---
id: T-153
type: task
title: Configure Next standalone output for packaging
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-001]
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: S-051
epic: E-014
owner: ""
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
tags: [frontend, packaging, next]
created: 2026-07-24
updated: 2026-07-29T11:30:07.936Z
started_at: 2026-07-28T08:31:48Z
completed_at: 2026-07-28T08:36:30Z
actual_ms: 47000
---

# T-153: Configure Next standalone output for packaging

## Description

Enable Next.js `output: 'standalone'` (or equivalent shippable build) so the UI can be bundled into an npm package without requiring consumers to run `next build` themselves.

## Acceptance criteria

- [x] Production build produces a standalone (or otherwise relocatable) server artifact.
- [x] Static assets required by the standalone server are included in the package layout plan.
- [x] Local `npm run build` still works for development of `taskmark-frontend`.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for zero-config npm/CLI board UI (no Docker) |
| 2 | 2026-07-28T08:31:48Z | prompt | Marco Mendão | Implement E-014 remaining stories: publishable npm CLI (taskmark serve, port 8275) and board-init one-command UI launch docs/stub |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T08:31:48Z | 2026-07-28T08:32:35.000Z | Next output standalone + prepare-standalone static assets; shared-batch: 47000 of 282000ms by points |
