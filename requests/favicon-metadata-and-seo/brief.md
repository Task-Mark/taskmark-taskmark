---
id: R-favicon-metadata-and-seo
type: request
title: Favicon, metadata, and SEO
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-28
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - frontend
  - website
  - branding
  - seo
  - favicon
aliases:
  - E-020
source_meetings: []
links: []
---

# Favicon, metadata, and SEO

## Goal

Ship consistent Taskmark brand icons and SEO/social metadata across the local board UI (`taskmark-frontend` / `@taskmark/ui`) and the marketing site (`taskmark-website`), including Open Graph images for link previews.

## Scope

- Install the provided favicon pack (apple-touch, ico/svg/png, web app manifests) into app `public/` trees and wire them in Next.js metadata.
- Expand title, description, theme color, and social (Open Graph / Twitter) metadata.
- Design and export Open Graph image(s) matching the TM inbox brand, then wire them in both apps.

## Done when

- Browser tab and “Add to Home Screen” show the new TM icons on local UI and website.
- Sharing a website URL (and optionally local UI docs if applicable) shows a branded Open Graph preview.
- `site.webmanifest` / icons resolve without 404s.

## Out of scope

- Changing product logos inside the in-app board chrome beyond favicon/metadata usage.
- Paid SEO tooling, sitemap generation beyond basic metadata, or multi-locale SEO.

## Open questions

_None yet._
