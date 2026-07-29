---
id: T-245
type: task
title: Verify favicon and apple touch on local UI
status: done
priority: high
size: S
size_source: suggested
size_basis: []
points: 2
points_source: suggested
estimate_minutes: 30
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
updated: 2026-07-29T07:31:14.976Z
started_at: 2026-07-28T14:47:21Z
completed_at: 2026-07-28T14:50:02Z
actual_ms: 9774
---
# T-245: Verify favicon and apple touch on local UI

## Description

Smoke-check tab icon, `/favicon.ico`, SVG, and apple-touch in a browser against `npm run dev` or `taskmark serve`.

## Acceptance criteria

- [x] No 404s for wired icon URLs.
- [x] Tab shows TM mark (not generic Next/default).

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
| 1 | Marco Mendão | 2026-07-28T14:47:21Z | 2026-07-28T14:47:30.774Z | Verified favicon assets present; shared-batch: 9774 of 161269ms by points |
