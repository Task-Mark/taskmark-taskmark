---
id: T-MM-4a7a944b
type: task
title: Keep version footers visible across Taskmark surfaces
status: done
priority: medium
size: S
points: 3
parent: S-003
epic: E-001
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
tags: [ui, footer, branding, website]
created: 2026-09-15
updated: 2026-09-15T20:37:36Z
started_at: 2026-09-15T18:10:46Z
completed_at: 2026-09-15T18:12:26Z
---
# T-MM-4a7a944b: Keep version footers visible across Taskmark surfaces

## Description

Refine the shared local and Cloud board footer into a low-profile fixed bar, and expose the latest Taskmark SemVer in the public website footer.

## User story

As a Taskmark user, I want the product version to remain unobtrusively visible on boards and appear on the website so I can quickly confirm which release each surface represents.

## Acceptance criteria

- [x] Local and Cloud boards use the same low-profile footer fixed to the bottom of the viewport.
- [x] Board content reserves enough space that the fixed footer does not cover it.
- [x] The public website footer shows the latest Taskmark version from its package metadata.
- [x] Relevant package checks pass.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T18:10:46Z | prompt | Marco Mendão | Keep a low-profile version footer fixed at the bottom of every local and Cloud board, and show the latest Taskmark version on the website footer. |
| 2026-09-15T20:37:36Z | feedback | Marco Mendão | Verify that the frontend and Cloud use the current shared footer dependency, resolve any stale installs, and ensure the website build completes cleanly. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T18:10:46Z | 2026-09-15T18:12:26Z | Made the shared board version footer fixed and compact with reserved content space, and added the package version to the website footer. |
| Marco Mendão | 2026-09-15T20:32:00Z | 2026-09-15T20:37:36Z | Confirmed frontend and Cloud use the linked 1.1.0 footer, fixed the website navigation type that blocked its build, and validated all three surfaces. |
