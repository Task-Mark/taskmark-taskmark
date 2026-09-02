---
id: E-MM-69ccb23d
type: epic
title: Shared UI component library
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
tags: [ui, design-system, cloud]
created: 2026-09-02
updated: 2026-09-02T07:51:50Z
started_at: null
completed_at: null
---
# E-MM-69ccb23d: Shared UI component library

## Description

Create a sibling `taskmark-ui` repository that owns Taskmark interface components, theme tokens, and presentational board building blocks for reuse by the local frontend, cloud app, and website.

## Goal

Keep Taskmark products visually consistent without copying interface code, while preserving `@taskmark/ui` as the local board application and CLI.

## Acceptance criteria

- [ ] A reusable `@taskmark/components` package exists in `taskmark-ui`.
- [ ] Frontend, cloud, and website consume the shared package.
- [ ] The local frontend keeps filesystem, CLI, and board-loading responsibilities outside the component package.
- [ ] All affected products build and lint successfully.
