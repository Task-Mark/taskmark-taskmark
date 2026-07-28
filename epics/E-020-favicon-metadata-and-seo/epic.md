---
id: E-020
type: epic
title: Favicon, metadata, and SEO
status: in_progress
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 36
points_source: rolled_up
estimate_minutes: 500
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
tags: [frontend, website, branding, seo, favicon]
created: 2026-07-28
updated: 2026-07-28T15:03:07.151Z
started_at: 2026-07-28T14:47:21Z
completed_at: null
actual_ms: 210420
---
# E-020: Favicon, metadata, and SEO

## Goal

Ship consistent Taskmark brand icons and SEO/social metadata across the local board UI (`taskmark-frontend` / `@taskmark/ui`) and the marketing site (`taskmark-website`), including Open Graph images for link previews.

## Scope

- Install the provided favicon pack (apple-touch, ico/svg/png, web app manifests) into app `public/` trees and wire them in Next.js metadata.
- Expand title, description, theme color, and social (Open Graph / Twitter) metadata.
- Design and export Open Graph image(s) matching the TM inbox brand, then wire them in both apps.

## Out of scope

- Changing product logos inside the in-app board chrome beyond favicon/metadata usage.
- Paid SEO tooling, sitemap generation beyond basic metadata, or multi-locale SEO.

## Success metrics

- Browser tab and “Add to Home Screen” show the new TM icons on local UI and website.
- Sharing a website URL (and optionally local UI docs if applicable) shows a branded Open Graph preview.
- `site.webmanifest` / icons resolve without 404s.

## Stories

- [S-080: Favicon pack for local board UI](stories/S-080-favicon-local-board-ui/story.md)
- [S-081: Favicon pack for marketing website](stories/S-081-favicon-marketing-website/story.md)
- [S-082: App metadata and SEO tags](stories/S-082-app-metadata-and-seo-tags/story.md)
- [S-083: Create Open Graph social images](stories/S-083-create-open-graph-images/story.md)
- [S-084: Wire Open Graph and Twitter cards](stories/S-084-wire-open-graph-twitter-cards/story.md)

## Tasks

- [T-255: Website favicon, metadata, and SEO parity](items/T-255-website-favicon-metadata-seo-parity.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-28T14:40:40Z | prompt | Marco Mendão | Create epic + stories/tasks for favicon pack, metadata/SEO, and Open Graph images |
| 2 | 2026-07-28T14:47:21Z | prompt | Marco Mendão | /start-work E-020 — implement favicon pack, metadata/SEO, and Open Graph |
| 3 | 2026-07-28T14:59:13Z | prompt | Marco Mendão | /create-task — same favicon and everything for Taskmark-website |
| 4 | 2026-07-28T15:02:18Z | prompt | Marco Mendão | start developing — website favicon/metadata/SEO parity |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 9b6ddcf | taskmark-website | 2026-07-28T15:14:29Z | Marco Mendão | add favicon metadata and seo |
| cee3f8d | taskmark-frontend | 2026-07-28T15:14:29Z | Marco Mendão | add favicon metadata and og images |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T14:47:21Z | 2026-07-28T14:47:21Z | Rollup: E-020 complete; billable on leaves (shared-batch); 0-min parent |
