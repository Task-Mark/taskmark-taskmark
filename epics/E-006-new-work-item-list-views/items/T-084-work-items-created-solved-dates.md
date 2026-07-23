---
id: T-084
type: task
title: Show created and solved dates on work items list
status: done
priority: medium
size: XS
size_source: suggested
size_basis: [calibrated:T-084]
points: 1
points_source: suggested
estimate_minutes: 20
actual_minutes: 21
estimate_source: suggested
estimate_basis: [calibrated:T-084]
session_cap_minutes: 480
parent: E-006
epic: E-006
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
tags: [dashboard, frontend, views, workitems, dates]
created: 2026-07-23
updated: 2026-07-23T17:36:48Z
started_at: 2026-07-23T07:46:42Z
completed_at: 2026-07-23T07:50:02Z
actual_ms: 1266000
---
# T-084: Show created and solved dates on work items list

## Description

Add creation date (`created`) and solve date (`completed_at`) columns to the Work items list table so users can see when each story or epic-direct task/bug was created and when it was completed.

## Acceptance criteria

- [x] Work items table shows a Created column from frontmatter `created`.
- [x] Work items table shows a Solved column from frontmatter `completed_at`.
- [x] Missing or empty dates display as an em dash.
- [x] Dates are readable in the list (date-focused, not raw noisy timestamps when avoidable).

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T07:46:42Z | prompt | Marco Mendão | Add solve date and creation date on the work items list |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 83d2ae9 | taskmark-frontend | 2026-07-23T08:04:28Z | Marco Mendão | add created solved date tooltips |
| 1cee199 | taskmark-taskmark | 2026-07-23T08:04:28Z | Marco Mendão | add t-084 t-085 date tooltip board |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T07:46:42Z | 2026-07-23T07:50:02Z | Added Created and Solved columns on work items list |
| 2 | Marco Mendão | 2026-07-23T07:46:42Z | 2026-07-23T08:04:28Z | auto-recovered: commit span |
