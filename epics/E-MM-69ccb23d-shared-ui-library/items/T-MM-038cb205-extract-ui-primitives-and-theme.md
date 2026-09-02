---
id: T-MM-038cb205
type: task
title: Extract UI primitives and theme
status: done
priority: high
size: L
points: 8
parent: E-MM-69ccb23d
epic: E-MM-69ccb23d
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
tags: [ui, theme]
created: 2026-09-02
updated: 2026-09-02T09:06:23Z
started_at: 2026-09-02T07:51:50Z
completed_at: 2026-09-02T08:14:16Z
---
# T-MM-038cb205: Extract UI primitives and theme

## Description

Move shared UI primitives, charts, theme tokens, providers, and brand components into `@taskmark/components`.

## Acceptance criteria

- [x] Shared primitives and charts are exported from the package.
- [x] Theme CSS, provider, toggle, toaster, logo, and utility helpers have one source of truth.
- [x] Package source contains no consumer-specific `@/` aliases.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T07:51:50Z | prompt | Marco Mendão | Extract the complete reusable Taskmark interface into a shared library. |
| 2026-09-02T09:06:23Z | feedback | Marco Mendão | Contact form fields looked wrong: text inputs kept the thin transparent variant instead of the thick bordered one, making them nearly invisible on dark backgrounds. |
| 2026-09-02T09:11:44Z | feedback | Marco Mendão | The brand mark was replaced by a drawn shape; the original image-based logo must be kept, even if each product ships its own copy of the image files. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T07:51:50Z | 2026-09-02T08:14:16Z | Extracted primitives, charts, theme, brand, and utility sources into the package. |
| Marco Mendão | 2026-09-02T09:00:00Z | 2026-09-02T09:06:23Z | Aligned shared text fields with the bordered design language so form inputs stay visible in both themes. |
| Marco Mendão | 2026-09-02T09:06:23Z | 2026-09-02T09:11:44Z | Restored the original image-based brand mark and shipped the brand images with the cloud product. |
