---
id: S-019
type: story
title: Load full work item content
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 10
points_source: rolled_up
estimate_minutes: 160
actual_minutes: 1
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-005
epic: E-005
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
tags: [dashboard, frontend, parse, detail]
created: 2026-07-21
updated: 2026-07-27T07:36:40.469Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 60938
---

# S-019: Load full work item content

## User story

As a user, I want the app to load every detail from a work item’s markdown so the sheet can show complete, accurate information.

## Acceptance criteria

- [x] Detail types cover frontmatter fields plus body sections for epics, stories, and tasks/bugs.
- [x] Epic, story, and task/bug markdown can be loaded by file path into typed detail models.
- [x] Shared section/table parsing covers goal/user story/description, AC, children lists, prompt & feedback, commits, and work log where present.
- [x] Parse failures for one file return a clear error without crashing the board.

## Tasks

- [T-051: Define detail types and shared section parsers](items/T-051-detail-types-shared-parsers.md)
- [T-052: Load epic full detail by file path](items/T-052-load-epic-full-detail.md)
- [T-053: Load story full detail by file path](items/T-053-load-story-full-detail.md)
- [T-054: Load task and bug full detail by file path](items/T-054-load-task-bug-full-detail.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T23:48:59Z | prompt | Marco Mendão | Create all user stories and tasks for E-005 view work item |
| 2 | 2026-07-21T23:53:57Z | prompt | Marco Mendão | Develop epic E-005 — implement work item detail views in sheets |
| 3 | 2026-07-21T23:56:38Z | feedback | Marco Mendão | Implement E-005 detail sheets delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T23:53:57Z | 2026-07-21T23:53:57Z | Delivered as part of E-005; shared-batch: 0ms rollup (children hold allocation) |
