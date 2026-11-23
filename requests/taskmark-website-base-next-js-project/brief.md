---
id: R-taskmark-website-base-next-js-project
type: request
title: Taskmark website base Next.js project
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-27
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - website
  - frontend
  - nextjs
  - docs
aliases:
  - E-017
source_meetings: []
links: []
---

# Taskmark website base Next.js project

## Goal

Stand up a new Next.js project for the public Taskmark website that reuses the same UI component stack and visual interface as `taskmark-frontend`, so later documentation and marketing pages can ship on a shared design system without rebuilding the app shell.

## Scope

- Create a sibling Next.js app (e.g. `taskmark-website`) aligned with `taskmark-frontend` versions and tooling (Next, React, Tailwind, TypeScript, ESLint).
- Port or share the frontend UI primitives, theme tokens, fonts, and layout/interface patterns needed for a marketing/docs site shell.
- Provide a working App Router layout, shared providers, and a placeholder homepage that proves the shared UI stack.
- Wire the new repo into the multi-project workspace so Taskmark board tooling can see it.

## Done when

- `taskmark-website` runs `dev` / `build` / `lint` successfully.
- Shared UI components and theme visibly match `taskmark-frontend`.
- Repo is a linked product root beside the other Taskmark projects.

## Out of scope

- Full documentation content, CMS, or markdown docs site structure beyond a smoke homepage.
- Blog, marketing campaigns, SEO content packs, analytics, or hosting/CDN deployment.
- Extracting a published shared UI package (local copy/port is enough for this epic).
- Changing `taskmark-frontend` board-app behavior.

## Open questions

_None yet._
