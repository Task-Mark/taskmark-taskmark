---
id: S-042
type: story
title: Initials avatars on work item lists
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 9
points_source: rolled_up
estimate_minutes: 140
actual_minutes: 2
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
tags: [identity, frontend, avatars, lists]
created: 2026-07-23
updated: 2026-07-27T06:17:22.249Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 120000
---
# S-042: Initials avatars on work item lists

## User story

As a board viewer, I want initials avatars on epic, story, and task lists for who reported and who resolved each item so I can see attribution at a glance.

## Acceptance criteria

- [x] Avatars render initials only (no photos); underlying data still has name, email, initials.
- [x] Epic, story, and task/bug lists show reporter and resolver avatars.
- [x] If the same person (same email) both created and resolved, show a single avatar.
- [x] Hover shows “Created by &lt;name&gt;”, “Resolved by &lt;name&gt;”, or “Created and developed by &lt;name&gt;” as appropriate.
- [x] Multiple distinct authors/resolvers show multiple avatars (stack or group).

## Tasks

- [T-119: Initials avatar component with hover tooltip](items/T-119-initials-avatar-component.md)
- [T-120: Parse reporters and resolvers in the frontend](items/T-120-parse-reporters-resolvers-frontend.md)
- [T-121: Show avatars on epic, story, and task lists](items/T-121-avatars-on-work-item-lists.md)
- [T-122: Multi-avatar stack and same-person dedupe](items/T-122-multi-avatar-dedupe.md)

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
