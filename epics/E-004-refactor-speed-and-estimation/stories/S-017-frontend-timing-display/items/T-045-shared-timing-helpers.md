---
id: T-045
type: task
title: Shared frontmatter timing field helpers
status: done
priority: high
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 120
actual_minutes: 0
estimate_basis: []
session_cap_minutes: 480
parent: S-017
epic: E-004
owner: ""
blocked: false
cancelled: false
tags: [frontend, estimation, actual]
created: 2026-07-21
updated: 2026-07-21T23:01:27Z
started_at: 2026-07-21T23:00:19Z
completed_at: 2026-07-21T23:01:18Z
---
# T-045: Shared frontmatter timing field helpers

## Description

Centralize reading estimate_minutes, actual_minutes, and optional effort_minutes from frontmatter for epic/story/item parsers.

## Acceptance criteria

- [x] Helper exports timing fields used by all three parsers.
- [x] estimate_minutes and actual_minutes always mapped.
- [x] effort_minutes optional.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T23:00:19Z | prompt | Ensure frontend keeps showing estimate and actual after latest Taskmark changes |
| 2 | 2026-07-21T23:01:18Z | feedback | timing display delivered |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T23:00:19Z | 2026-07-21T23:01:18Z | Frontend timing display hardened for flat boards |
