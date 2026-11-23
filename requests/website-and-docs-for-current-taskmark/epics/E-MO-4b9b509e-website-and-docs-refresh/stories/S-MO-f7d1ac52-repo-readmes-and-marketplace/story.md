---
id: S-MO-f7d1ac52
type: story
title: Repo READMEs and marketplace copy
status: backlog
priority: medium
size: S
points: 3
parent: E-MO-4b9b509e
epic: E-MO-4b9b509e
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [docs, readme]
created: 2026-08-28
updated: 2026-08-28T23:15:25Z
started_at: null
completed_at: null
---

# S-MO-f7d1ac52: Repo READMEs and marketplace copy

## User story

As a contributor cloning the workspace, I want Cursor, frontend, website, and board-root READMEs (and marketplace blurb) to describe the same four commands and board layout so I am not sent to a generated Last-synced dashboard.

## Acceptance criteria

- [ ] `taskmark-cursor` and plugin READMEs stay aligned with `/tkmd-*`, leaf-only writes, static sizing, and no INDEX/SIZING/VELOCITY/board README.
- [ ] Workspace/board-root README no longer publishes Last synced, Current speed, or a generated open-work changelog as product documentation.
- [ ] `taskmark-frontend` README remains accurate for `@taskmark/ui` install/serve and does not revive retired slash commands.
- [ ] `taskmark-website` README points at landing + docs without contradicting the four-command model.
- [ ] Cursor marketplace plugin description matches the four focused commands if it is user-visible.
