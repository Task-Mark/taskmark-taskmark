---
id: S-084
type: story
title: Wire Open Graph and Twitter cards
status: done
priority: medium
size: M
size_source: rolled_up
size_basis: [sum:tasks]
points: 6
points_source: rolled_up
estimate_minutes: 80
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
tags: [frontend, website, seo, opengraph]
created: 2026-07-28
updated: 2026-07-29T06:48:27.505Z
started_at: 2026-07-28T14:47:21Z
completed_at: 2026-07-28T14:50:02Z
actual_ms: 29321
---
# S-084: Wire Open Graph and Twitter cards

## User story

As a sharer of Taskmark URLs, I want Open Graph and Twitter card tags to resolve to the branded image and correct title/description.

## Acceptance criteria

- [x] Website metadata includes `openGraph` and `twitter` with image, title, description.
- [x] Local UI sets OG/Twitter reasonably (even if rarely shared) or documents local-only limitation.
- [x] Preview validators (or manual curl of meta tags) show absolute image URLs on the website.

## Tasks

- [T-253: Wire Open Graph and Twitter on website](items/T-253-wire-og-twitter-website.md)
- [T-254: Wire Open Graph and Twitter on local board UI](items/T-254-wire-og-twitter-frontend.md)

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
