---
id: S-MM-9956e0ef
type: story
title: Public GitHub repository and npm library for shared UI
status: backlog
priority: high
size: null
points: null
parent: E-MM-69ccb23d
epic: E-MM-69ccb23d
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [ui, npm, github]
created: 2026-09-15
updated: 2026-09-15T11:16:00Z
started_at: null
completed_at: null
---
# S-MM-9956e0ef: Public GitHub repository and npm library for shared UI

## Description

Treat `taskmark-ui` as a public GitHub repository and publish `@taskmark/components` as a public scoped npm package, so consumers and Cloud CI can use it without a private checkout token.

## User story

As a Taskmark product developer, I want the shared UI library to be public on GitHub and npm so I can install it like any other open package and build Cloud images without a PAT for `taskmark-ui`.

## Acceptance criteria

- [ ] `@taskmark/components` is configured for a public npm publish.
- [ ] CI can publish the package to the public npm registry.
- [ ] The Cloud ECR workflow checks out `Task-Mark/taskmark-ui` without `UI_REPO_TOKEN`.
