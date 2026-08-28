---
id: S-062
type: story
title: Scaffold Taskmark website Next.js project
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 7
points_source: rolled_up
estimate_minutes: 100
actual_minutes: 1
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
tags: [website, nextjs, scaffolding]
created: 2026-07-27
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-07-27T09:54:28Z
completed_at: 2026-07-27T09:56:34Z
actual_ms: 60000
---
# S-062: Scaffold Taskmark website Next.js project

## User story

As a Taskmark contributor, I want a dedicated Next.js website project scaffolded beside the existing repos with the same core toolchain as `taskmark-frontend`, so we can build docs and marketing pages without forking the board UI app.

## Acceptance criteria

- [x] A sibling `taskmark-website` (or agreed name) Next.js app exists with Next/React versions aligned to `taskmark-frontend`.
- [x] TypeScript, ESLint, PostCSS, and Tailwind configs mirror the frontend project conventions.
- [x] The website repo is initialized as git and discoverable as a linked product root in the Taskmark workspace.

## Tasks

- [T-196: Create sibling Next.js app with matching Next and React versions](items/T-196-create-sibling-nextjs-app-with-matching-next-and-react-versions.md)
- [T-197: Align TypeScript ESLint Tailwind and PostCSS with frontend](items/T-197-align-typescript-eslint-tailwind-and-postcss-with-frontend.md)
- [T-198: Initialize git and link website repo in workspace REPOS](items/T-198-initialize-git-and-link-website-repo-in-workspace-repos.md)

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
