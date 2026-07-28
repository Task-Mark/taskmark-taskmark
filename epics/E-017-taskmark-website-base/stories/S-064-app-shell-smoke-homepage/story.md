---
id: S-064
type: story
title: App shell providers and smoke homepage
status: done
priority: medium
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 5
points_source: rolled_up
estimate_minutes: 75
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-017
epic: E-017
owner: ""
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
tags: [website, app-router, smoke]
created: 2026-07-27
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-27T09:54:28Z
completed_at: 2026-07-27T09:56:34Z
actual_ms: 0
---
# S-064: App shell providers and smoke homepage

## User story

As a contributor, I want a working App Router shell with shared providers and a placeholder homepage, so I can verify the website stack end-to-end before adding documentation content.

## Acceptance criteria

- [x] Root layout wires shared theme (and any required) providers.
- [x] A placeholder homepage renders using shared UI components.
- [x] `dev`, `build`, and `lint` succeed on the website project.

## Tasks

- [T-202: Wire App Router root layout with shared theme providers](items/T-202-wire-app-router-root-layout-with-shared-theme-providers.md)
- [T-203: Build placeholder homepage using shared UI components](items/T-203-build-placeholder-homepage-using-shared-ui-components.md)
- [T-204: Verify dev build and lint scripts succeed](items/T-204-verify-dev-build-and-lint-scripts-succeed.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 2 | 2026-07-27T09:54:28Z | prompt | Marco Mendão | Implement E-017 website base Next.js project |
| 1 | 2026-07-27T07:56:00Z | prompt | Marco Mendão | Create epic + stories/tasks for Taskmark website Next.js base sharing frontend UI |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| fa6cb40 | taskmark-website | 2026-07-28T06:19:03Z | Marco Mendão | scaffold taskmark website |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T09:54:28Z | 2026-07-27T09:54:28Z | E-017 shared-batch: 0min rollup (children hold allocation) |
