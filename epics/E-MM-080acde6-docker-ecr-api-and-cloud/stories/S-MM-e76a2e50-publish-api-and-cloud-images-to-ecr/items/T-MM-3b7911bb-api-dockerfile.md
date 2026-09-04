---
id: T-MM-3b7911bb
type: task
title: Add a production Dockerfile for the API
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
tags: [api, docker]
created: 2026-09-04
updated: 2026-09-04T08:57:27Z
started_at: 2026-09-04T08:42:00Z
completed_at: 2026-09-04T08:57:27Z
---
# T-MM-3b7911bb: Add a production Dockerfile for the API

## Description

Add a multi-stage Dockerfile and `.dockerignore` in `taskmark-api` so `docker build -t taskmark/api .` produces a production Node image that runs `node dist/main.js` on port 4000. Do not copy `.env` into the image.

## Acceptance criteria

- [x] `docker build -t taskmark/api .` from `taskmark-api` succeeds.
- [x] The image starts the Nest app on port 4000 with runtime env (Mongo, JWT, Cloud URL).
- [x] `.env` and `node_modules` are not copied into the build context.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-04T08:42:00Z | prompt | Marco Mendão | Add Docker images for API and Cloud and a GitHub pipeline to publish them to ECR (`dev` from development, `latest` from main). |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Marco Mendão | 2026-09-04T08:42:00Z | 2026-09-04T08:57:27Z | Added a multi-stage API Dockerfile and confirmed docker build -t taskmark/api . |
