---
id: T-MM-392d4d3a
type: task
title: Add board theme toggle using the shared cookie
status: done
priority: medium
size: M
points: 5
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
tags: [frontend, theme, cookie]
created: 2026-08-29
updated: 2026-08-29T19:04:16Z
started_at: 2026-08-29T18:49:00Z
completed_at: 2026-08-29T18:52:50Z
---

# T-MM-392d4d3a: Add board theme toggle using the shared cookie

## Description

Give the board UI a light/dark control in the app bar. Default to the operating system until the user chooses. Persist the choice in the same `taskmark_theme` cookie as the website so changing theme on either surface is used by the other.

## Acceptance criteria

- [x] The board app bar includes a control that switches between light and dark on live and static board chrome.
- [x] With no theme cookie, the board uses `prefers-color-scheme`.
- [x] Choosing light or dark applies immediately, writes `taskmark_theme`, and is restored on later visits.
- [x] On `taskmark.dev` hosts the cookie uses `Domain=.taskmark.dev`; brand logos and existing dark tokens follow the resolved theme.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T18:48:30Z | prompt | Marco Mendão | Board and website should share a light/dark toggle; default to OS; persist in a cookie used by both. |
| 2026-08-29T19:04:16Z | feedback | Marco Mendão | The board background stayed light in dark mode. |
| 2026-08-29T19:04:16Z | prompt | Marco Mendão | Fix the dark-theme background on the board. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T18:49:00Z | 2026-08-29T18:52:50Z | Board ThemeProvider, app-bar toggle, cookie tests and lint. |
| Marco Mendão | 2026-08-29T19:00:00Z | 2026-08-29T19:04:16Z | Themed board surfaces: base body colors, token gradients, card metrics; lint and tests. |
