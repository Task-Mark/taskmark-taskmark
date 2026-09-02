---
id: T-MM-e9e5aafa
type: task
title: Configure NestJS MongoDB models and HTTP hardening
status: done
priority: high
size: L
points: 8
parent: S-MM-0dda88f5
epic: E-MM-63bde04a
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
tags: [api, mongodb]
created: 2026-09-02
updated: 2026-09-02T15:52:15Z
started_at: 2026-09-02T15:28:10Z
completed_at: 2026-09-02T15:52:15Z
---
# T-MM-e9e5aafa: Configure NestJS MongoDB models and HTTP hardening

## Description

Switch the API scaffold to npm, add validated configuration, connect Mongoose, define the auth domain schemas, and apply `/v1` plus Helmet, CORS, validation, and rate limiting.

## Acceptance criteria

- [x] Required env is validated at boot and documented in `.env.example` without secrets.
- [x] User, project, membership, invitation, verification, and refresh-session models exist.
- [x] The API listens under `/v1` with Helmet, CORS, ValidationPipe, and rate limiting.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | From the Cloud Auth Registration plan: prepare NestJS, MongoDB, validated config, and multi-tenant models. |
| 2026-09-02T15:28:10Z | prompt | Marco Mendão | `/tkmd-save-do`: implement this leaf without committing or pushing. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T15:28:10Z | 2026-09-02T15:52:15Z | Switched the API to npm, validated env, added Mongoose models, and hardened HTTP under `/v1`. |
