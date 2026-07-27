---
id: T-121
type: task
title: Show avatars on epic, story, and task lists
status: done
priority: high
size: M
size_source: suggested
size_basis: [velocity:similar]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 1
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
tags: [frontend, avatars, lists]
created: 2026-07-23
updated: 2026-07-27T05:18:44.416Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 60000
---

# T-121: Show avatars on epic, story, and task lists

## Description

Render reporter/resolver avatars on epic, story, and task/bug list rows (Overall drill-down and Work items table as applicable).

## Acceptance criteria

- [x] Epic list rows show attribution avatars when identities exist.
- [x] Story list rows show attribution avatars when identities exist.
- [x] Task/bug list rows show attribution avatars when identities exist.
- [x] Empty identity shows no avatar clutter (or a subtle placeholder only if design requires).

## Notes

Wire through the shared avatar + dedupe helpers from T-119/T-122.

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
| 1 | Marco Mendão | 2026-07-23T17:31:57Z | 2026-07-23T17:32:57Z | delivered; shared-batch: 1 of 8min by points |
