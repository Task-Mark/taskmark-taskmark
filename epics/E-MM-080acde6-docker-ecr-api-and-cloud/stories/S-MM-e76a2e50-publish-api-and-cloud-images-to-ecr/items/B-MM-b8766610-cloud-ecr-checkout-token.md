---
id: B-MM-b8766610
type: bug
title: Cloud ECR workflow fails UI checkout without a token
status: done
priority: high
size: S
points: 3
parent: S-MM-e76a2e50
epic: E-MM-080acde6
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
tags: [cloud, ecr, github-actions]
created: 2026-09-04
updated: 2026-09-04T15:28:53Z
started_at: 2026-09-04T15:25:00Z
completed_at: 2026-09-04T15:28:53Z
---
# B-MM-b8766610: Cloud ECR workflow fails UI checkout without a token

## Description

The Cloud publish workflow checks out `Task-Mark/taskmark-ui` with `secrets.UI_REPO_TOKEN`. When that secret is unset, `actions/checkout@v4` receives an empty token and fails with `Input required and not supplied: token`. The same job also warns that Node 20 is deprecated on GitHub-hosted runners.

## Fix criteria

- [x] Checking out `taskmark-ui` does not fail with `Input required and not supplied: token` when `UI_REPO_TOKEN` is empty.
- [x] The workflow uses GitHub Actions that run on Node 24 (no Node 20 deprecation from `actions/checkout`).
- [x] A missing `UI_REPO_TOKEN` is reported with a clear instruction to add a PAT that can read `Task-Mark/taskmark-ui`.
- [x] When `UI_REPO_TOKEN` is set, the job still checks out Cloud and UI into sibling directories for the parent Docker context.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-04T15:25:00Z | prompt | Marco Mendão | Cloud GitHub pipeline fails on `actions/checkout@v4` of `Task-Mark/taskmark-ui` with `Input required and not supplied: token`, plus a Node 20 deprecation warning. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 119d73e133484a18908d9623fc6660483fa2d6be | taskmark-cloud | 2026-09-04T15:29:59Z | Marco Mendão | add production compose and fix worklog import |
| 5c455370fb83021e5a7e32b26892684c47b186ae | taskmark-taskmark | 2026-09-04T15:29:59Z | Marco Mendão | sync taskmark board |

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-04T15:25:00Z | 2026-09-04T15:28:53Z | Bumped Cloud ECR actions to Node 24 runtimes and fail fast when UI_REPO_TOKEN is missing instead of passing an empty checkout token |
