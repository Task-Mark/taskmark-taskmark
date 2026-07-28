---
id: E-017
type: epic
title: Taskmark website base Next.js project
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 20
points_source: rolled_up
estimate_minutes: 285
actual_minutes: 3
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
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
tags: [website, frontend, nextjs, docs]
created: 2026-07-27
updated: 2026-07-28T15:31:09.902Z
started_at: 2026-07-27T09:54:28Z
completed_at: 2026-07-27T09:56:34Z
actual_ms: 180000
---
# E-017: Taskmark website base Next.js project

## Goal

Stand up a new Next.js project for the public Taskmark website that reuses the same UI component stack and visual interface as `taskmark-frontend`, so later documentation and marketing pages can ship on a shared design system without rebuilding the app shell.

## Scope

- Create a sibling Next.js app (e.g. `taskmark-website`) aligned with `taskmark-frontend` versions and tooling (Next, React, Tailwind, TypeScript, ESLint).
- Port or share the frontend UI primitives, theme tokens, fonts, and layout/interface patterns needed for a marketing/docs site shell.
- Provide a working App Router layout, shared providers, and a placeholder homepage that proves the shared UI stack.
- Wire the new repo into the multi-project workspace so Taskmark board tooling can see it.

## Out of scope

- Full documentation content, CMS, or markdown docs site structure beyond a smoke homepage.
- Blog, marketing campaigns, SEO content packs, analytics, or hosting/CDN deployment.
- Extracting a published shared UI package (local copy/port is enough for this epic).
- Changing `taskmark-frontend` board-app behavior.

## Success metrics

- `taskmark-website` runs `dev` / `build` / `lint` successfully.
- Shared UI components and theme visibly match `taskmark-frontend`.
- Repo is a linked product root beside the other Taskmark projects.

## Stories

- [S-062: Scaffold Taskmark website Next.js project](stories/S-062-scaffold-website-nextjs/story.md)
- [S-063: Share UI components and visual interface with frontend](stories/S-063-share-ui-with-frontend/story.md)
- [S-064: App shell providers and smoke homepage](stories/S-064-app-shell-smoke-homepage/story.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| fa6cb40 | taskmark-website | 2026-07-28T06:19:03Z | Marco Mendão | scaffold taskmark website |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T09:54:28Z | 2026-07-27T09:54:28Z | E-017 website base shipped; shared-batch: 0min rollup (children hold allocation) |
