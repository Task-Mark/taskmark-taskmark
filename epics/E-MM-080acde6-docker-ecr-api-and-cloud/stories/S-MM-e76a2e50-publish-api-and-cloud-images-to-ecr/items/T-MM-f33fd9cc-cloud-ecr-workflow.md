---
id: T-MM-f33fd9cc
type: task
title: Publish the Cloud image to ECR from GitHub Actions
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
updated: 2026-09-04T08:57:27Z
started_at: 2026-09-04T08:42:00Z
completed_at: 2026-09-04T08:57:27Z
---
# T-MM-f33fd9cc: Publish the Cloud image to ECR from GitHub Actions

## Description

Add a workflow on `taskmark-cloud` that checks out Cloud and `Task-Mark/taskmark-ui`, builds with the Cloud Dockerfile from a parent context, logs in to ECR, and pushes `taskmark/cloud:dev` or `taskmark/cloud:latest` from `development` / `main`.

## Acceptance criteria

- [x] Push to `development` pushes `394754814010.dkr.ecr.eu-central-1.amazonaws.com/taskmark/cloud:dev`.
- [x] Push to `main` pushes `394754814010.dkr.ecr.eu-central-1.amazonaws.com/taskmark/cloud:latest`.
- [x] The build context includes `taskmark-ui` so the file dependency resolves.
- [x] Login uses AWS credentials from repository secrets, not hardcoded keys.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-04T08:42:00Z | prompt | Marco Mendão | Add Docker images for API and Cloud and a GitHub pipeline to publish them to ECR (`dev` from development, `latest` from main). |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Marco Mendão | 2026-09-04T08:42:00Z | 2026-09-04T08:57:27Z | Added the Cloud GitHub Action that checks out UI, builds from the parent context, and pushes to ECR |
