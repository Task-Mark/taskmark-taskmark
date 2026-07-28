---
id: T-156
type: task
title: Document npx and npm start usage
status: done
priority: medium
size: S
size_source: suggested
size_basis: [T-030]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:15min/pt]
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
tags: [frontend, packaging, docs]
created: 2026-07-24
updated: 2026-07-28T14:32:06.722Z
started_at: 2026-07-28T08:31:48Z
completed_at: 2026-07-28T08:36:30Z
actual_ms: 31334
---

# T-156: Document npx and npm start usage

## Description

Write package README (and/or frontend README section) with the primary happy path `npx taskmark serve` on port **8275**, plus local install + script wrappers, env overrides, and cwd expectations for nested vs flat boards.

## Acceptance criteria

- [x] Docs lead with `npx taskmark serve` and `http://localhost:8275`.
- [x] Docs show the happy path from product root and from board root.
- [x] Env vars `TASKMARK_BOARD` / `TASKMARK_MASTER` (and port override) are documented.
- [x] Setup-wizard fallback (cookie mode) is mentioned for multi-master use.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-24T17:26:00Z | prompt | Marco Mendão | Create epic + stories/tasks for zero-config npm/CLI board UI (no Docker) |
| 2 | 2026-07-25T10:21:15Z | prompt | Marco Mendão | CLI must be `npx taskmark serve`; default port 8275 |
| 3 | 2026-07-28T08:31:48Z | prompt | Marco Mendão | Implement E-014 remaining stories: publishable npm CLI (taskmark serve, port 8275) and board-init one-command UI launch docs/stub |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T08:31:48Z | 2026-07-28T08:32:19.334Z | Frontend README documents npx taskmark serve @ 8275; shared-batch: 31334 of 282000ms by points |
