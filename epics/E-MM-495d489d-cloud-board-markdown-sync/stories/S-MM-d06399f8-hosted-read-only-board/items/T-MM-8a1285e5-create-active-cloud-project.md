---
id: T-MM-8a1285e5
type: task
title: Create active cloud projects for signed-in users
status: done
priority: high
size: M
points: 5
parent: S-MM-d06399f8
epic: E-MM-495d489d
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
tags: [cloud, api, projects]
created: 2026-09-03
updated: 2026-09-03T14:31:58Z
started_at: 2026-09-03T14:28:14Z
completed_at: 2026-09-03T14:31:58Z
---
# T-MM-8a1285e5: Create active cloud projects for signed-in users

## Description

Add an authenticated API operation that creates an active project with a unique slug and an active owner membership for the current user.

## Acceptance criteria

- [x] A signed-in user can create a project with a non-empty name.
- [x] The project receives a unique slug and is active immediately.
- [x] The creator receives an active owner membership and the project appears in the next `/auth/me` response.
- [x] Unauthenticated and invalid requests are rejected, with end-to-end coverage.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-03T14:28:14Z | prompt | Marco Mendão | Add a cloud board project picker that also lets the signed-in user create a new associated project. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-03T14:28:14Z | 2026-09-03T14:31:58Z | Added authenticated project creation with validation, unique slugs, active owner membership, and end-to-end coverage. |
