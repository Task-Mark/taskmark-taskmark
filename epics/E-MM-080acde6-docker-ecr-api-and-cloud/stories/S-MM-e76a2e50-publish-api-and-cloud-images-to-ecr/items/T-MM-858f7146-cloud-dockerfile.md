---
id: T-MM-858f7146
type: task
title: Add a production Dockerfile for Cloud
status: done
priority: high
size: M
points: 5
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
tags: [cloud, docker]
created: 2026-09-04
updated: 2026-09-04T08:57:27Z
started_at: 2026-09-04T08:42:00Z
completed_at: 2026-09-04T08:57:27Z
---
# T-MM-858f7146: Add a production Dockerfile for Cloud

## Description

Add a Dockerfile for `taskmark-cloud` that builds Next.js in standalone mode with the sibling `taskmark-ui` package (`file:../taskmark-ui`). The build context is the parent of both folders so `docker build -f taskmark-cloud/Dockerfile -t taskmark/cloud .` from the workspace (or the CI layout) works. Do not copy `.env` into the image; `API_URL` is runtime env.

## Acceptance criteria

- [x] Cloud builds with `@taskmark/components` from the sibling UI package.
- [x] The image runs `next start` / standalone on port 3000.
- [x] `.env` files are not copied into the image.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-04T08:42:00Z | prompt | Marco Mendão | Add Docker images for API and Cloud and a GitHub pipeline to publish them to ECR (`dev` from development, `latest` from main). |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Marco Mendão | 2026-09-04T08:42:00Z | 2026-09-04T08:57:27Z | Added a Cloud Dockerfile with sibling UI install and confirmed docker build -t taskmark/cloud |
