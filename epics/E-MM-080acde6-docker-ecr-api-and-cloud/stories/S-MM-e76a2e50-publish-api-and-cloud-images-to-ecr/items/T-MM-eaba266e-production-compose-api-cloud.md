---
id: T-MM-eaba266e
type: task
title: Add production Compose for API and Cloud
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
tags: [docker, compose, cloud, api]
created: 2026-09-04
updated: 2026-09-04T09:11:02Z
started_at: 2026-09-04T09:08:00Z
completed_at: 2026-09-04T09:11:02Z
---
# T-MM-eaba266e: Add production Compose for API and Cloud

## Description

Add a Docker Compose file on the production host layout that pulls the ECR API and Cloud images and runs them together. Cloud talks to API on the Compose network. Mongo stays external via `MONGODB_URI`. Secrets come from an env file, not from the images.

## Acceptance criteria

- [x] Compose starts `api` and `cloud` from the ECR images with a configurable `dev` or `latest` tag.
- [x] Cloud reaches the API over the internal network; the public port is Cloud only.
- [x] Required secrets are documented in an example env file and are not hardcoded.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-04T09:08:00Z | prompt | Marco Mendão | Create a docker compose file that runs the API and Cloud together on the production machine. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Marco Mendão | 2026-09-04T09:08:00Z | 2026-09-04T09:11:02Z | Added production Compose that pulls API and Cloud from ECR and proxies Cloud to the API internally. |
