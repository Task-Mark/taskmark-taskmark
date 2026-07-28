---
id: T-113
type: task
title: Git config identity helper (name, email, initials)
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
tags: [identity, git, plugin, scripts]
created: 2026-07-23
updated: 2026-07-28T07:27:54.696Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 0
---

# T-113: Git config identity helper (name, email, initials)

## Description

Add a plugin script/helper that reads local `git config user.name` and `user.email` (repo-local then global) and returns `{ name, email, initials }`.

## Acceptance criteria

- [x] Helper returns name, email, and derived initials when git config is set.
- [x] Missing config returns a safe empty/null result without crashing callers.
- [x] Helper is usable from create/complete skills and README sync.

## Notes

Prefer running git in the active product/board repo; fall back to global config.

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
