---
id: T-124
type: task
title: Show authors on Work log
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
tags: [work-log, identity, plugin, frontend]
created: 2026-07-23
updated: 2026-07-25T10:24:50.747Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 60000
---
# T-124: Show authors on Work log

## Description

Stamp Work log Actor with the current git identity (name) when starting/completing sessions, and show that identity in the UI so multiple developers are visible across sessions.

## Acceptance criteria

- [x] start-work / complete-work write Actor using git user name when available.
- [x] Frontend Work log displays the actor identity clearly.
- [x] Different sessions can show different authors.

## Notes

May keep a role tag like `agent` in summary while Actor holds the human git name.

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
| 1 | Marco Mendão | 2026-07-23T17:34:57Z | 2026-07-23T17:35:57Z | delivered; shared-batch: 1 of 8min by points |
