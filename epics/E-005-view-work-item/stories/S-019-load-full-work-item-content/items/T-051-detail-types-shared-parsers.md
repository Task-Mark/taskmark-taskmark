---
id: T-051
type: task
title: Define detail types and shared section parsers
status: done
priority: high
size: M
size_source: suggested
size_basis: [calibrated:T-051]
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
tags: [parse, frontend, detail]
created: 2026-07-21
updated: 2026-07-22T00:16:21.562Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 18281
---
# T-051: Define detail types and shared section parsers

## Description

Add typed models for full work item details and shared helpers to parse markdown sections and markdown tables (commits, work log, prompt & feedback, AC checklists).

## Acceptance criteria

- [x] Detail types exist for epic, story, and task/bug beyond list summary fields.
- [x] Shared helpers can extract named `##` sections and markdown tables into structured data.
- [x] Acceptance-criteria style checklists can be parsed into items with checked state when present.
- [x] Helpers fail gracefully with useful errors on malformed input.

## Notes

Extend existing frontmatter/timing parsers; avoid duplicating list-summary parsing.

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
