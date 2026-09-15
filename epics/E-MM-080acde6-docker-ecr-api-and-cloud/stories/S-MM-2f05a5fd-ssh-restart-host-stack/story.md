---
id: S-MM-2f05a5fd
type: story
title: Restart host Docker stack over SSH after ECR publish
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
tags: [docker, ci, ssh, deploy]
created: 2026-09-15
updated: 2026-09-15T11:43:00Z
started_at: null
completed_at: null
---
# S-MM-2f05a5fd: Restart host Docker stack over SSH after ECR publish

## Description

After API or Cloud images are pushed to ECR, SSH into the production host and recreate the Compose stack in `/var/apps/taskmark` so it pulls the new images.

## User story

As someone deploying Taskmark, I want a successful ECR publish to restart the Docker stack on the host so I do not have to log in and pull images by hand.

## Acceptance criteria

- [ ] Cloud and API publish workflows SSH to the host after a successful image push.
- [ ] The remote command runs in `/var/apps/taskmark` and refreshes the Compose stack.
- [ ] Host and key come from GitHub secrets, not from the workflow file.
