---
id: T-112
type: task
title: Add reporters and resolvers frontmatter on work items
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
parent: S-039
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
tags: [identity, frontmatter, templates]
created: 2026-07-23
updated: 2026-08-17T08:03:41.619Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 0
---
# T-112: Add reporters and resolvers frontmatter on work items

## Description

Extend epic/story/task/bug templates and frontmatter so each item can store `reporters` and `resolvers` as lists of identity objects (`name`, `email`, `initials`).

## Acceptance criteria

- [x] Templates include empty `reporters: []` and `resolvers: []` (or equivalent YAML).
- [x] Frontmatter reference documents the fields for all work-item types.
- [x] Existing items without the fields remain parseable (default to empty lists).

## Notes

`owner` may remain for now; reporters/resolvers are the attribution source of truth for this epic.

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
| 1 | Marco Mendão | 2026-07-23T17:28:57Z | 2026-07-23T17:28:57Z | delivered; shared-batch: 0 of 8min by points |
