---
id: T-051
type: task
title: Define detail types and shared section parsers
status: backlog
priority: high
size: M
size_source: suggested
size_basis: [T-014, T-005]
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
tags: [parse, frontend, detail]
created: 2026-07-21
updated: 2026-07-21T23:50:12Z
started_at: null
completed_at: null
---

# T-051: Define detail types and shared section parsers

## Description

Add typed models for full work item details and shared helpers to parse markdown sections and markdown tables (commits, work log, prompt & feedback, AC checklists).

## Acceptance criteria

- [ ] Detail types exist for epic, story, and task/bug beyond list summary fields.
- [ ] Shared helpers can extract named `##` sections and markdown tables into structured data.
- [ ] Acceptance-criteria style checklists can be parsed into items with checked state when present.
- [ ] Helpers fail gracefully with useful errors on malformed input.

## Notes

Extend existing frontmatter/timing parsers; avoid duplicating list-summary parsing.

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
