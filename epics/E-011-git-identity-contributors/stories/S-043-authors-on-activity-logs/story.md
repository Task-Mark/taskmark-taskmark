---
id: S-043
type: story
title: Authors on activity logs
status: done
priority: medium
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 6
points_source: rolled_up
estimate_minutes: 90
actual_minutes: 3
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-011
epic: E-011
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
tags: [identity, commits, work-log, prompt-feedback, frontend, plugin]
created: 2026-07-23
updated: 2026-07-23T17:36:48Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 180000
---
# S-043: Authors on activity logs

## User story

As a board viewer, I want authors visible on the Commits list, Work log, and Prompt & feedback so I can see who contributed each activity entry — including when multiple people are involved.

## Acceptance criteria

- [x] Commits table shows commit author (from git author / logged identity).
- [x] Work log rows show the human git identity (not only generic `agent`) when available.
- [x] Prompt & feedback rows record and display the author identity.
- [x] UI and markdown support multiple authors associated with an item’s activity over time.

## Tasks

- [T-123: Show authors on Commits table](items/T-123-authors-on-commits.md)
- [T-124: Show authors on Work log](items/T-124-authors-on-work-log.md)
- [T-125: Show authors on Prompt and feedback](items/T-125-authors-on-prompt-feedback.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T17:28:57Z | prompt | Marco Mendão | Start developing E-011 (story scope). |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T17:28:57Z | 2026-07-23T17:28:57Z | rollup: children hold shared-batch; delivered story |
