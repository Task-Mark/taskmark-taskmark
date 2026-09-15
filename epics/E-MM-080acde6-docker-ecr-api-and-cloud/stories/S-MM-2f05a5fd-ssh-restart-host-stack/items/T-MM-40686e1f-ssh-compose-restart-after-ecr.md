---
id: T-MM-40686e1f
type: task
title: SSH into the host and recreate Compose after ECR push
status: done
priority: high
size: S
points: 3
parent: S-MM-2f05a5fd
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
tags: [docker, ci, ssh]
created: 2026-09-15
updated: 2026-09-15T11:46:00Z
started_at: 2026-09-15T11:43:00Z
completed_at: 2026-09-15T11:46:00Z
---
# T-MM-40686e1f: SSH into the host and recreate Compose after ECR push

## Description

Add a post-push step to the Cloud and API ECR workflows that SSHs to the host and runs Compose pull plus up in `/var/apps/taskmark`.

## Acceptance criteria

- [x] Both publish workflows fail fast when `SSH_HOST`, `SSH_USER`, or `SSH_PRIVATE_KEY` is missing.
- [x] After a successful image push they SSH and run Compose in `/var/apps/taskmark`.
- [x] Connection details are only read from repository secrets.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T11:43:00Z | prompt | Marco Mendão | After ECR publish, SSH into the machine and restart Docker in /var/apps/taskmark. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T11:43:00Z | 2026-09-15T11:46:00Z | Added SSH Compose pull and up in /var/apps/taskmark to the Cloud and API ECR publish workflows. |
