---
id: T-MM-8ee5e974
type: task
title: Collapse the website header navigation into a mobile hamburger menu
status: done
priority: medium
size: S
points: 3
parent: S-MO-60c97eed
epic: E-MO-4b9b509e
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
tags: [website, navigation, mobile]
created: 2026-08-31
updated: 2026-08-31T11:26:45Z
started_at: 2026-08-31T11:24:50Z
completed_at: 2026-08-31T11:26:45Z
---

# T-MM-8ee5e974: Collapse the website header navigation into a mobile hamburger menu

## Description

On small screens the website header links wrap onto a second line. On mobile the header must show only the brand logo and a hamburger button; every header link and control moves into the menu that button opens.

## Acceptance criteria

- [x] On mobile widths the header shows only the brand and a hamburger button, and never wraps onto a second row.
- [x] The menu opened by the hamburger button contains every header destination and control available on desktop.
- [x] Choosing a destination in the menu navigates and closes the menu.
- [x] Desktop and larger widths keep the current inline header navigation unchanged.
- [x] The hamburger button and menu are keyboard reachable and labelled for screen readers.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T11:24:50Z | prompt | Marco Mendão | On mobile the website navigation bar should be a hamburger menu holding every header link, leaving only the logo and the hamburger icon so the bar never takes two rows. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T11:24:50Z | 2026-08-31T11:26:45Z | Shared header link list, sheet-based mobile menu with theme toggle and start CTA, single-row header; typecheck, lint, and production build. |
