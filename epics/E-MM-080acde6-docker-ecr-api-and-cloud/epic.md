---
id: E-MM-080acde6
type: epic
title: Docker images and ECR publish for API and Cloud
status: backlog
priority: high
size: null
points: null
parent: null
epic: null
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [docker, ecr, ci, cloud, api]
created: 2026-09-04
updated: 2026-09-04T08:42:00Z
started_at: null
completed_at: null
---
# E-MM-080acde6: Docker images and ECR publish for API and Cloud

## Description

Ship production Docker images for `taskmark-api` and `taskmark-cloud`, and publish them to Amazon ECR in `eu-central-1` from GitHub Actions. `development` maps to the `dev` image tag; `main` maps to `latest`.

## Goal

A push to `development` or `main` builds and pushes `taskmark/api` and `taskmark/cloud` to `394754814010.dkr.ecr.eu-central-1.amazonaws.com` with the branch tag rules above.

## Acceptance criteria

- [ ] API and Cloud each have a production Dockerfile that can be built without secrets in the image.
- [ ] GitHub Actions on each product repo authenticates to ECR and pushes the matching repository.
- [ ] `development` publishes `:dev`; `main` publishes `:latest`.
