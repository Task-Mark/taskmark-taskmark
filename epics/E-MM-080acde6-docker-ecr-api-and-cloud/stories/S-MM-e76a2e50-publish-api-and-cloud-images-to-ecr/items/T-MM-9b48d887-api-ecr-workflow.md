---
id: T-MM-9b48d887
type: task
title: Publish the API image to ECR from GitHub Actions
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
tags: [api, ecr, github-actions]
created: 2026-09-04
updated: 2026-09-04T08:57:27Z
started_at: 2026-09-04T08:42:00Z
completed_at: 2026-09-04T08:57:27Z
---
# T-MM-9b48d887: Publish the API image to ECR from GitHub Actions

## Description

Add a workflow on `taskmark-api` that on push to `development` or `main` logs in to `394754814010.dkr.ecr.eu-central-1.amazonaws.com` with GitHub AWS secrets, builds `taskmark/api`, and pushes `…/taskmark/api:dev` or `…/taskmark/api:latest`.

## Acceptance criteria

- [x] Push to `development` pushes `394754814010.dkr.ecr.eu-central-1.amazonaws.com/taskmark/api:dev`.
- [x] Push to `main` pushes `394754814010.dkr.ecr.eu-central-1.amazonaws.com/taskmark/api:latest`.
- [x] Login uses AWS credentials from repository secrets, not hardcoded keys.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-04T08:42:00Z | prompt | Marco Mendão | Add Docker images for API and Cloud and a GitHub pipeline to publish them to ECR (`dev` from development, `latest` from main). |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Marco Mendão | 2026-09-04T08:42:00Z | 2026-09-04T08:57:27Z | Added the API GitHub Action that logs in to ECR and pushes dev or latest |
