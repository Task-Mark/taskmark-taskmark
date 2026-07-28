---
id: T-118
type: task
title: Sync README when a new git identity appears
status: done
priority: medium
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
parent: S-041
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
tags: [contributors, readme, plugin]
created: 2026-07-23
updated: 2026-07-28T09:08:49.505Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 0
---

# T-118: Sync README when a new git identity appears

## Description

Hook create/complete (or a small sync step) so when a new git identity is stamped on a work item, the README Contributors section is updated automatically.

## Acceptance criteria

- [x] First time a new email is stamped, README gains that contributor.
- [x] Subsequent stamps for the same email do not rewrite unnecessarily.
- [x] Skill/script documents when sync runs.

## Notes

Can reuse the upsert helper from T-117.

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
