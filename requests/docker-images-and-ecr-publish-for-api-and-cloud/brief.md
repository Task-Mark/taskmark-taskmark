---
id: R-docker-images-and-ecr-publish-for-api-and-cloud
type: request
title: Docker images and ECR publish for API and Cloud
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-09-04
updated: 2026-09-04T08:42:00Z
forecast: null
tags:
  - docker
  - ecr
  - ci
  - cloud
  - api
aliases:
  - E-MM-080acde6
source_meetings: []
links: []
---

# Docker images and ECR publish for API and Cloud

## Goal

A push to `development` or `main` builds and pushes `taskmark/api` and `taskmark/cloud` to `394754814010.dkr.ecr.eu-central-1.amazonaws.com` with the branch tag rules above.

## Done when

- [ ] API and Cloud each have a production Dockerfile that can be built without secrets in the image.
- [ ] GitHub Actions on each product repo authenticates to ECR and pushes the matching repository.
- [ ] `development` publishes `:dev`; `main` publishes `:latest`.

## Out of scope

_Nothing yet._

## Open questions

_None yet._
