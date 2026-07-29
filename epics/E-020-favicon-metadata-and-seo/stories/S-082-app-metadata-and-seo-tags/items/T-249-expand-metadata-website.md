---
id: T-249
type: task
title: Expand Next metadata for marketing website
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 40
actual_minutes: 0
estimate_source: suggested
estimate_basis: [speed:90d:14min/pt]
session_cap_minutes: 480
parent: S-082
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
tags: [frontend, website, seo, metadata]
created: 2026-07-28
updated: 2026-07-29T07:31:14.976Z
started_at: 2026-07-28T14:47:21Z
completed_at: 2026-07-28T14:50:02Z
actual_ms: 14661
---
# T-249: Expand Next metadata for marketing website

## Description

Improve website root metadata: title template, description, `metadataBase`, themeColor, and any robots/canonical defaults appropriate for a public site.

## Acceptance criteria

- [x] `metadataBase` is set to the production site origin (configurable via env if needed).
- [x] Title template remains `%s · Taskmark` or equivalent.

## Notes

Source favicon pack (provided): `taskmark-frontend/public/favicon (4)/` — apple-touch-icon.png, favicon-96x96.png, favicon.ico, favicon.svg, site.webmanifest, web-app-manifest-192x192.png, web-app-manifest-512x512.png.

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
| 1 | Marco Mendão | 2026-07-28T14:47:21Z | 2026-07-28T14:47:35.661Z | Expanded website metadataBase + SEO; shared-batch: 14661 of 161269ms by points |
