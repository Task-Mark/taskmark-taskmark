---
id: T-MM-e95e8f5f
type: task
title: Persist website theme in the shared Taskmark cookie
status: done
priority: medium
size: S
points: 3
parent: S-MM-2da610bb
epic: E-001
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
tags: [website, theme, cookie]
created: 2026-08-29
updated: 2026-08-29T18:52:50Z
started_at: 2026-08-29T18:49:00Z
completed_at: 2026-08-29T18:52:50Z
---

# T-MM-e95e8f5f: Persist website theme in the shared Taskmark cookie

## Description

Keep the existing website light/dark header control. Stop relying on origin-only storage for the chosen theme. Write and read a shared cookie so the hosted board can use the same preference. Until the visitor chooses, keep following the operating system.

## Acceptance criteria

- [x] With no theme cookie, the website still uses `prefers-color-scheme`.
- [x] Choosing light or dark updates the page immediately and writes cookie `taskmark_theme` (`light` or `dark` only).
- [x] On `taskmark.dev` and `*.taskmark.dev`, the cookie is set with `Domain=.taskmark.dev` so the hosted board can read it.
- [x] Returning to the website restores the chosen theme from that cookie (no flash back to the opposite OS theme when a cookie is present).

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T18:48:30Z | prompt | Marco Mendão | Board and website should share a light/dark toggle; default to OS; persist in a cookie used by both. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T18:49:00Z | 2026-08-29T18:52:50Z | Shared `taskmark_theme` cookie, init script, ThemeCookieSync; website lint. |
