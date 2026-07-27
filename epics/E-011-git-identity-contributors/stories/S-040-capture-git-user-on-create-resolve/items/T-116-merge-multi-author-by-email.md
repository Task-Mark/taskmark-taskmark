---
id: T-116
type: task
title: Merge multi-author identity lists by email
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
parent: S-040
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
tags: [identity, plugin]
created: 2026-07-23
updated: 2026-07-27T07:06:27.645Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 0
---
# T-116: Merge multi-author identity lists by email

## Description

Shared merge utility: append an identity into `reporters` or `resolvers` without duplicating the same email; update name/initials if the existing entry is incomplete.

## Acceptance criteria

- [x] Same email is not listed twice in reporters or resolvers.
- [x] Different emails accumulate as multiple authors/developers.
- [x] Case-insensitive email compare.

## Notes

Used by create, complete-work, README sync, and log-commits paths.

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
| 1 | Marco Mendão | 2026-07-23T17:30:57Z | 2026-07-23T17:30:57Z | delivered; shared-batch: 0 of 8min by points |
