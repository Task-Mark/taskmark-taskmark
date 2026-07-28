---
id: S-056
type: story
title: Project contributors view
status: done
priority: medium
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 70
actual_minutes: 1
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-015
epic: E-015
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
tags: [frontend, contributors, identity]
created: 2026-07-27
updated: 2026-07-28T07:27:54.696Z
started_at: 2026-07-27T06:25:20Z
completed_at: 2026-07-27T06:28:48Z
actual_ms: 60000
---

# S-056: Project contributors view

## User story

As a project lead, I want a simple view of everyone who has contributed to the project board, so I can see who is involved without scanning every work item.

## Acceptance criteria

- [x] Collect unique contributors from board work-item `reporters` and `resolvers` (dedupe by email).
- [x] Optionally merge README Contributors when already parsed — do not invent new identity sources.
- [x] Simple view shows initials avatars plus name (and email on hover or secondary text).
- [x] Empty state when no identities are present yet.
- [x] Placed near the metrics strip so status + people read as one project overview.

## Tasks

- [T-175: Collect unique project contributors](items/T-175-collect-project-contributors.md)
- [T-176: Build contributors panel UI](items/T-176-contributors-panel-ui.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 2 | 2026-07-27T06:25:20Z | prompt | Marco Mendão | Implement the E-015 |
| 1 | 2026-07-27T05:55:45Z | prompt | Marco Mendão | Create epic for project status metrics (total/complete/speed + contributors) styled like neo-brutalism metric cards; include stories and tasks |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:25:20Z | 2026-07-27T06:25:20Z | Parent rollup: children hold shared-batch |
