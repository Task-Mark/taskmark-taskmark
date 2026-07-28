---
id: T-114
type: task
title: Stamp reporter on create-* skills
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
tags: [identity, plugin, create]
created: 2026-07-23
updated: 2026-07-28T06:20:01.202Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 60000
---
# T-114: Stamp reporter on create-* skills

## Description

Update `create-epic`, `create-story`, and `create-task` so newly created items include the current git identity in `reporters`.

## Acceptance criteria

- [x] New epics, stories, tasks, and bugs get the current git user in `reporters`.
- [x] Skills docs mention stamping reporter from git config.
- [x] Create still succeeds when git identity is unavailable (empty reporters).

## Notes

Also seed activity author where Prompt & feedback / Work log rows are written at create time if applicable.

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
| 1 | Marco Mendão | 2026-07-23T17:28:57Z | 2026-07-23T17:29:57Z | delivered; shared-batch: 1 of 8min by points |
