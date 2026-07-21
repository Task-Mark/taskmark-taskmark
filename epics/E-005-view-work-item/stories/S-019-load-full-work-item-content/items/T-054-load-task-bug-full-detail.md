---
id: T-054
type: task
title: Load task and bug full detail by file path
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-014, T-015]
points: 3
points_source: suggested
estimate_minutes: 50
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-019
epic: E-005
owner: ""
blocked: false
cancelled: false
tags: [parse, frontend, tasks]
created: 2026-07-21
updated: 2026-07-21T23:50:12Z
started_at: null
completed_at: null
---

# T-054: Load task and bug full detail by file path

## Description

Load and parse full task and bug detail models from item markdown paths, including type-specific sections (description/AC vs description/repro/fix criteria), notes, prompt & feedback, commits, and work log.

## Acceptance criteria

- [ ] Given a task or bug file path, returns a typed item detail or a clear parse error.
- [ ] Distinguishes task vs bug section shapes.
- [ ] Includes frontmatter fields needed for the sheet header/meta.
- [ ] Missing optional sections do not fail the whole parse.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T23:48:59Z | prompt | Create all user stories and tasks for E-005 view work item |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
