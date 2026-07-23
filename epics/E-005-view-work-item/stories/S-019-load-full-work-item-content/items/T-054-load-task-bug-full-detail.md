---
id: T-054
type: task
title: Load task and bug full detail by file path
status: done
priority: high
size: M
size_source: suggested
size_basis: [calibrated:T-054]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_source: manual
estimate_basis: [manual:preserve-plan;burst-delivery]
session_cap_minutes: 480
parent: S-019
epic: E-005
owner: ""
blocked: false
cancelled: false
tags: [parse, frontend, tasks]
created: 2026-07-21
updated: 2026-07-23T09:47:44.562Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 18281
---
# T-054: Load task and bug full detail by file path

## Description

Load and parse full task and bug detail models from item markdown paths, including type-specific sections (description/AC vs description/repro/fix criteria), notes, prompt & feedback, commits, and work log.

## Acceptance criteria

- [x] Given a task or bug file path, returns a typed item detail or a clear parse error.
- [x] Distinguishes task vs bug section shapes.
- [x] Includes frontmatter fields needed for the sheet header/meta.
- [x] Missing optional sections do not fail the whole parse.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T23:48:59Z | prompt | Create all user stories and tasks for E-005 view work item |
| 2 | 2026-07-21T23:56:38Z | feedback | Implement E-005 detail sheets delivered |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T23:53:57Z | 2026-07-21T23:54:15.281Z | Delivered as part of E-005; shared-batch: 18281 of 195000ms by points |
