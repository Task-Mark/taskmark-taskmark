---
id: S-080
type: story
title: Favicon pack for local board UI
status: done
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 7
points_source: rolled_up
estimate_minutes: 100
actual_minutes: 0
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-020
epic: E-020
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
tags: [frontend, branding, favicon]
created: 2026-07-28
updated: 2026-07-29T06:48:27.505Z
started_at: 2026-07-28T14:47:21Z
completed_at: 2026-07-28T14:50:02Z
actual_ms: 34209
---
# S-080: Favicon pack for local board UI

## User story

As a developer using the local board UI, I want the browser tab and PWA icons to show the Taskmark TM brand so the app looks finished and recognizable.

## Acceptance criteria

- [x] Provided favicon assets live under `taskmark-frontend/public/` (not the temporary `favicon (4)/` folder name).
- [x] Root layout `metadata.icons` (and apple) point at the new assets.
- [x] `site.webmanifest` is published and icon paths resolve (200).

## Tasks

- [T-243: Install favicon assets into frontend public](items/T-243-install-favicon-assets-frontend.md)
- [T-244: Wire favicon and webmanifest in frontend layout](items/T-244-wire-favicon-layout-frontend.md)
- [T-245: Verify favicon and apple touch on local UI](items/T-245-verify-favicon-frontend.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-28T14:40:40Z | prompt | Marco Mendão | Create epic + stories/tasks for favicon pack, metadata/SEO, and Open Graph images |
| 2 | 2026-07-28T14:47:21Z | prompt | Marco Mendão | /start-work E-020 — implement favicon, metadata, OG |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T14:47:21Z | 2026-07-28T14:47:21Z | Rollup: E-020 delivery; 0-min parent |
