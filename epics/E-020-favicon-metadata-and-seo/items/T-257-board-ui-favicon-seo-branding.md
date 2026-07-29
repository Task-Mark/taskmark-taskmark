---
id: T-257
type: task
title: Ship favicon and SEO branding in board folder web UI
status: done
priority: high
size: M
size_source: suggested
size_basis: []
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 4
estimate_source: suggested
estimate_basis: [calibrated:T-257]
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
tags: [frontend, branding, favicon, seo, board]
created: 2026-07-29
updated: 2026-07-29T06:48:27.505Z
started_at: 2026-07-29T05:47:29Z
completed_at: 2026-07-29T06:02:31Z
actual_ms: 254000
---

# T-257: Ship favicon and SEO branding in board folder web UI

## Description

Ensure the web UI for the Taskmark **board folder project** (`taskmark-taskmark` / `@taskmark/ui`) exposes the same favicon pack, app metadata, webmanifest branding, and Open Graph / Twitter cards already shipped for the local frontend and marketing site (E-020). Icons and meta must work when opening the board UI locally and when the board is hosted.

## Acceptance criteria

- [x] Board UI (`@taskmark/ui`) tab icon, apple-touch, and webmanifest resolve without 404s.
- [x] Title, description, theme color, and SEO-relevant metadata match Taskmark brand (parity with website / local frontend).
- [x] Open Graph / Twitter card tags and default OG image are present in the board UI document head.
- [x] Published / built board UI package includes favicon and social assets (not only source `public/` during `next dev`).

## Notes

Related: S-080–S-084, T-255 (website parity). Board project consumers should not need a separate favicon install.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 2 | 2026-07-29T05:47:29Z | prompt | Marco Mendão | implement everything you created (T-257–T-259) |
| 1 | 2026-07-29T05:40:31Z | prompt | Marco Mendão | Favicon and branding SEO should be in the board folder web UI |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-29T05:47:29Z | 2026-07-29T05:51:43Z | shared-batch: favicon/SEO metadataBase + assets in standalone/static |
