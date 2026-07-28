---
id: T-117
type: task
title: Upsert Contributors section in project README
status: done
priority: medium
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
updated: 2026-07-28T08:37:10.649Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 60000
---

# T-117: Upsert Contributors section in project README

## Description

Add or update a Contributors section in the relevant project README(s) listing contributor name and email from board identities.

## Acceptance criteria

- [x] README Contributors section lists name (and email when available).
- [x] Upsert is idempotent by email.
- [x] Target README(s) for this workspace are defined (e.g. product + board README).

## Notes

Prefer a clearly marked generated block so hand-written README content is not clobbered.

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
| 1 | Marco Mendão | 2026-07-23T17:30:57Z | 2026-07-23T17:31:57Z | delivered; shared-batch: 1 of 8min by points |
