---
id: T-153
type: task
title: Configure Next standalone output for packaging
status: backlog
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
resolvers: []
blocked: false
cancelled: false
tags: [frontend, packaging, next]
created: 2026-07-24
updated: 2026-07-28T07:27:54.696Z
started_at: null
completed_at: null
actual_ms: 0
---

# T-153: Configure Next standalone output for packaging

## Description

Enable Next.js `output: 'standalone'` (or equivalent shippable build) so the UI can be bundled into an npm package without requiring consumers to run `next build` themselves.

## Acceptance criteria

- [ ] Production build produces a standalone (or otherwise relocatable) server artifact.
- [ ] Static assets required by the standalone server are included in the package layout plan.
- [ ] Local `npm run build` still works for development of `taskmark-frontend`.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for zero-config npm/CLI board UI (no Docker) |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
