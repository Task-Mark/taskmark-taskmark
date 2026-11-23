---
id: S-MM-ff4c8a9b
type: story
title: Init writes a static project README
status: backlog
priority: high
size: null
points: null
parent: E-MO-4b9b509e
epic: E-MO-4b9b509e
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [docs, readme, init, plugin]
created: 2026-08-29
updated: 2026-08-29T17:25:00Z
started_at: null
completed_at: null
---

# S-MM-ff4c8a9b: Init writes a static project README

## User story

As someone running `/tkmd-init`, I want a static project README that explains what Taskmark is, which git products belong to this workspace, and how to run, build, and deploy the board (including Vercel, Docker, and `npx @taskmark/ui`) so I can start without a generated dashboard or the marketing site.

## Acceptance criteria

- [ ] `/tkmd-init` creates or repairs a **static** project README (not INDEX/SIZING/VELOCITY, not Last synced / Current speed / open-work changelog, not `CHANGELOG.md`)
- [ ] The README states Taskmark’s purpose, lists the workspace’s product repositories, and documents local run, build, Vercel, Docker, and standalone `npx @taskmark/ui`
- [ ] Board storage still has no generated dashboard README; conventions and the init command no longer forbid a static project README
