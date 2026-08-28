---
id: T-244
type: task
title: Wire favicon and webmanifest in frontend layout
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
parent: S-080
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
updated: 2026-08-28T12:37:43.783Z
started_at: 2026-07-28T14:47:21Z
completed_at: 2026-07-28T14:50:02Z
actual_ms: 14661
---

# T-244: Wire favicon and webmanifest in frontend layout

## Description

Update `app/layout.tsx` metadata icons (icon, shortcut, apple) and link/manifest for the local board UI.

## Acceptance criteria

- [x] `metadata.icons` no longer points only at `/tm_light.png` for primary favicon.
- [x] Manifest referenced for installable/PWA icon set.

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
| 1 | Marco Mendão | 2026-07-28T14:47:21Z | 2026-07-28T14:47:35.661Z | Wired frontend icons + metadata icons; shared-batch: 14661 of 161269ms by points |
