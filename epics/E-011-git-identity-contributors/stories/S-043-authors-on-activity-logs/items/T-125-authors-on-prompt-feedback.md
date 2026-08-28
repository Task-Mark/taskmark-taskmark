---
id: T-125
type: task
title: Show authors on Prompt and feedback
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
tags: [prompt-feedback, identity, plugin, frontend]
created: 2026-07-23
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 60000
---
# T-125: Show authors on Prompt and feedback

## Description

Extend Prompt & feedback log rows to record the author (git identity) and display authors in the work-item UI, supporting multiple people over time.

## Acceptance criteria

- [x] Prompt & feedback table includes Author (or equivalent) when rows are appended.
- [x] start-work / feedback append paths stamp current git identity.
- [x] Frontend shows author on Prompt & feedback entries.

## Notes

Align column naming with Commits/Work log conventions.

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
| 1 | Marco Mendão | 2026-07-23T17:35:57Z | 2026-07-23T17:36:57Z | delivered; shared-batch: 1 of 8min by points |
