---
id: T-053
type: task
title: Load story full detail by file path
status: backlog
priority: high
size: S
size_source: suggested
size_basis: [T-011, T-005]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-019
epic: E-005
owner: ""
blocked: false
cancelled: false
tags: [parse, frontend, stories]
created: 2026-07-21
updated: 2026-07-21T23:50:12Z
started_at: null
completed_at: null
---

# T-053: Load story full detail by file path

## Description

Load and parse a full story detail model from a `story.md` path, including user story, acceptance criteria, tasks, prompt & feedback, commits, work log, and frontmatter meta.

## Acceptance criteria

- [ ] Given a story file path, returns a typed story detail or a clear parse error.
- [ ] Includes frontmatter fields needed for the sheet header/meta.
- [ ] Includes body sections relevant to stories when present.
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
