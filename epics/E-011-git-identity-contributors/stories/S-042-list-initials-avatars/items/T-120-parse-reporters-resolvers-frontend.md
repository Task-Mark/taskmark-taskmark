---
id: T-120
type: task
title: Parse reporters and resolvers in the frontend
status: done
priority: high
size: S
size_source: suggested
size_basis: [velocity:similar]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-042
epic: E-011
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
tags: [frontend, identity, parsing]
created: 2026-07-23
updated: 2026-07-27T05:16:43.229Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 0
---
# T-120: Parse reporters and resolvers in the frontend

## Description

Extend work-item parsing so list/detail models include `reporters` and `resolvers` with name, email, and initials (derive initials client-side if missing).

## Acceptance criteria

- [x] Parsed epic/story/task models expose reporters and resolvers arrays.
- [x] Missing fields default to empty arrays.
- [x] Initials filled when only name is present.

## Notes

Keep types shared across Overall and Work items list views.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T17:28:57Z | prompt | Marco Mendão | User asked to start developing epic E-011. |
| 2 | 2026-07-23T17:36:57Z | feedback | Marco Mendão | Delivered identity schema, git helper, README sync, list avatars, activity authors. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T17:31:57Z | 2026-07-23T17:31:57Z | delivered; shared-batch: 0 of 8min by points |
