---
id: T-052
type: task
title: Load epic full detail by file path
status: done
priority: high
size: S
size_source: suggested
size_basis: [calibrated:T-052]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 3
estimate_source: manual
estimate_basis: [manual:preserve-plan;burst-delivery]
session_cap_minutes: 480
parent: S-019
epic: E-005
owner: ""
blocked: false
cancelled: false
tags: [parse, frontend, epic]
created: 2026-07-21
updated: 2026-07-21T23:57:22Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
---
# T-052: Load epic full detail by file path

## Description

Load and parse a full epic detail model from an `epic.md` path, including goal/scope/out of scope/success metrics/stories/commits/work log and frontmatter meta.

## Acceptance criteria

- [x] Given an epic file path, returns a typed epic detail or a clear parse error.
- [x] Includes frontmatter fields needed for the sheet header/meta.
- [x] Includes body sections relevant to epics when present.
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
| 1 | agent | 2026-07-21T23:53:57Z | 2026-07-21T23:57:12Z | Delivered T-052 as part of E-005 |
