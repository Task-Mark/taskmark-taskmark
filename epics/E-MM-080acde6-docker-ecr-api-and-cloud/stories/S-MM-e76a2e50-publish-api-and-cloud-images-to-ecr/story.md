---
id: S-MM-e76a2e50
type: story
title: Publish API and Cloud images to ECR
status: backlog
priority: high
size: null
points: null
parent: E-MM-080acde6
epic: E-MM-080acde6
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [docker, ecr, github-actions]
created: 2026-09-04
updated: 2026-09-04T08:42:00Z
started_at: null
completed_at: null
---
# S-MM-e76a2e50: Publish API and Cloud images to ECR

## Description

Add Dockerfiles for the Nest API and the Next.js Cloud app, then GitHub Actions that log in to `394754814010.dkr.ecr.eu-central-1.amazonaws.com` and push `taskmark/api` and `taskmark/cloud`. Cloud’s image must include the sibling `@taskmark/components` package. Branch `development` tags `dev`; branch `main` tags `latest`.

## User story

As someone deploying Taskmark Cloud, I want API and Cloud images in ECR so I can roll out `dev` from `development` and `latest` from `main` without building by hand.

## Acceptance criteria

- [ ] `taskmark-api` builds to a runnable image exposing the Nest port.
- [ ] `taskmark-cloud` builds to a runnable Next.js image and includes `@taskmark/components`.
- [ ] Pushing `development` updates the `dev` tag; pushing `main` updates `latest`.
- [ ] Workflows use AWS credentials from GitHub secrets and do not bake `.env` files into the image.
