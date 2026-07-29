---
id: T-255
type: task
title: Website favicon, metadata, and SEO parity
status: done
priority: high
size: XS
size_source: suggested
size_basis: [calibrated:T-255]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 16
estimate_source: suggested
estimate_basis: [calibrated:T-255]
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
tags: [website, branding, favicon, seo]
created: 2026-07-28
updated: 2026-07-29T07:31:14.976Z
started_at: 2026-07-28T14:47:21Z
completed_at: 2026-07-28T15:18:30Z
actual_ms: 972000
---
# T-255: Website favicon, metadata, and SEO parity

## Description

Apply the same favicon pack, app metadata/SEO tags, webmanifest branding, and Open Graph / Twitter cards to `taskmark-website` as shipped for the local board UI (`taskmark-frontend` / `@taskmark/ui`).

Umbrella for website parity already delivered under S-081 / S-082 / S-084 (T-246, T-247, T-249, T-250, T-253) and OG assets (T-251/T-252).

## Acceptance criteria

- [x] Website `public/` has the TM favicon pack (ico/svg/png, apple-touch, web-app manifests) with stable paths.
- [x] Website root layout wires icons, manifest, theme color, title/description, Open Graph, and Twitter cards.
- [x] `metadataBase` / site URL configured for absolute social preview URLs.
- [x] Default OG image (`public/og/og-default.png`) present and referenced.
- [x] Tab / home-screen / link-preview brand matches the product UI.

## Notes

Shipped in `taskmark-website` (`9b6ddcf`); assets match frontend.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-28T14:59:13Z | prompt | Marco Mendão | /create-task — same favicon and everything for Taskmark-website |
| 2 | 2026-07-28T15:02:18Z | prompt | Marco Mendão | start developing — website favicon/metadata/SEO parity |
| 3 | 2026-07-28T15:18:30Z | feedback | Marco Mendão | /complete-work — website favicon/SEO parity accepted |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 9b6ddcf | taskmark-website | 2026-07-28T15:14:29Z | Marco Mendão | add favicon metadata and seo |
| cee3f8d | taskmark-frontend | 2026-07-28T15:14:29Z | Marco Mendão | add favicon metadata and og images |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T14:47:21Z | 2026-07-28T14:47:21Z | Already delivered with E-020 website leaves; 0-min (no double-count) |
| 2 | Marco Mendão | 2026-07-28T15:02:18Z | 2026-07-28T15:18:30Z | Verified website favicon/metadata/SEO parity; committed 9b6ddcf |
