---
id: T-205
type: task
title: Remove Est and Actual columns from Overall lists
status: done
priority: medium
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 2
estimate_source: suggested
estimate_basis: [speed:90d:14min/pt]
session_cap_minutes: 480
parent: S-025
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
tags: [dashboard, frontend, overall, lists]
created: 2026-07-28
updated: 2026-07-28T06:20:01.202Z
started_at: 2026-07-28T06:14:00Z
completed_at: 2026-07-28T06:16:13Z
actual_ms: 133000
---
# T-205: Remove Est and Actual columns from Overall lists

## Description

Drop Est and Actual time columns from Overall drill-down tables (epic, story, and task lists). Timing remains available on the work-item detail sheet.

## Acceptance criteria

- [x] Epic Overall list has no Est or Actual columns
- [x] Story Overall list has no Est or Actual columns
- [x] Task/bug Overall list has no Est or Actual columns
- [x] Detail sheet still shows Est and Actual

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-28T06:14:00Z | prompt | Marco Mendão | Remove the columns Est, Actual from the lists on overall |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| cb6c435 | taskmark-frontend | 2026-07-28T06:18:39Z | Marco Mendão | remove overall est actual columns |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T06:14:00Z | 2026-07-28T06:16:13Z | Removed Est/Actual columns from Overall epic, story, and task lists |
