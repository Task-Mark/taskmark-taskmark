---
id: T-123
type: task
title: Show authors on Commits table
status: done
priority: medium
size: S
size_source: suggested
size_basis: [velocity:similar]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 1
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-043
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
tags: [commits, identity, plugin, frontend]
created: 2026-07-23
updated: 2026-07-28T19:13:32.846Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 60000
---

# T-123: Show authors on Commits table

## Description

Ensure Commits log rows include author (name/email from git commit author or logged identity) in markdown and display that author in the work-item UI.

## Acceptance criteria

- [x] `log-commits` (or equivalent) records author on each Commits row.
- [x] Commits table template/docs include an Author column (or equivalent).
- [x] Frontend detail view shows commit authors.

## Notes

Multiple commits can have different authors over the life of an item.

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
| 1 | Marco Mendão | 2026-07-23T17:33:57Z | 2026-07-23T17:34:57Z | delivered; shared-batch: 1 of 8min by points |
