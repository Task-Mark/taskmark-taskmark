---
id: T-MM-0699e98a
type: task
title: Checkout public taskmark-ui in Cloud ECR without a PAT
status: done
priority: high
size: S
points: 3
parent: S-MM-9956e0ef
epic: E-MM-69ccb23d
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
tags: [cloud, ci, github]
created: 2026-09-15
updated: 2026-09-15T11:20:00Z
started_at: 2026-09-15T11:16:00Z
completed_at: 2026-09-15T11:20:00Z
---
# T-MM-0699e98a: Checkout public taskmark-ui in Cloud ECR without a PAT

## Description

Stop requiring `UI_REPO_TOKEN` in the Cloud ECR workflow. Check out public `Task-Mark/taskmark-ui` with the default GitHub token.

## Acceptance criteria

- [x] The Cloud publish workflow does not read or require `secrets.UI_REPO_TOKEN`.
- [x] `actions/checkout` for `Task-Mark/taskmark-ui` omits an explicit token.
- [x] Cloud and UI still land in sibling directories for the parent Docker context.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T11:14:00Z | prompt | Marco Mendão | Taskmark UI should be a public repository and a public library on npm; make the changes needed for that to be true. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T11:16:00Z | 2026-09-15T11:20:00Z | Removed the UI_REPO_TOKEN guard so Cloud checks out taskmark-ui as a public sibling for the Docker parent context. |
