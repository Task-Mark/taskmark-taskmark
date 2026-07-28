---
id: T-196
type: task
title: Create sibling Next.js app with matching Next and React versions
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 1
estimate_source: suggested
estimate_basis: [speed:90d:14min/pt]
session_cap_minutes: 480
parent: S-062
epic: E-017
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
tags: [website, nextjs, scaffolding]
created: 2026-07-27
updated: 2026-07-28T07:27:54.696Z
started_at: 2026-07-27T09:54:28Z
completed_at: 2026-07-27T09:55:28Z
actual_ms: 60000
---
# T-196: Create sibling Next.js app with matching Next and React versions

## Description

Scaffold a new Next.js App Router project as a sibling of `taskmark-frontend`, using the same Next and React major versions from the frontend `package.json`.

## Acceptance criteria

- [x] Project directory exists with `package.json` naming the website app.
- [x] Next and React dependency versions match `taskmark-frontend` majors.
- [x] `npm`/`yarn` install completes without errors.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 2 | 2026-07-27T09:54:28Z | prompt | Marco Mendão | Implement E-017 website base Next.js project |
| 1 | 2026-07-27T07:56:00Z | prompt | Marco Mendão | Create epic + stories/tasks for Taskmark website Next.js base sharing frontend UI |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| fa6cb40 | taskmark-website | 2026-07-28T06:19:03Z | Marco Mendão | scaffold taskmark website |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T09:54:28Z | 2026-07-27T09:55:28Z | Delivered with E-017 batch; shared-batch: 1 of 3min by points |
