---
id: T-053
type: task
title: Load story full detail by file path
status: done
priority: high
size: S
size_source: suggested
size_basis: [calibrated:T-053]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: manual
estimate_basis: [manual:preserve-plan;burst-delivery]
session_cap_minutes: 480
parent: S-019
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
tags: [parse, frontend, stories]
created: 2026-07-21
updated: 2026-07-27T07:09:18.868Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 12188
---

# T-053: Load story full detail by file path

## Description

Load and parse a full story detail model from a `story.md` path, including user story, acceptance criteria, tasks, prompt & feedback, commits, work log, and frontmatter meta.

## Acceptance criteria

- [x] Given a story file path, returns a typed story detail or a clear parse error.
- [x] Includes frontmatter fields needed for the sheet header/meta.
- [x] Includes body sections relevant to stories when present.
- [x] Missing optional sections do not fail the whole parse.

## Notes

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-21T23:48:59Z | prompt | Marco Mendão | Create all user stories and tasks for E-005 view work item |
| 2 | 2026-07-21T23:56:38Z | feedback | Marco Mendão | Implement E-005 detail sheets delivered |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-21T23:53:57Z | 2026-07-21T23:54:09.188Z | Delivered as part of E-005; shared-batch: 12188 of 195000ms by points |
