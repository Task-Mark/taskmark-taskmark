---
id: T-MM-7be25985
type: task
title: Add light/dark theme switcher on the website
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
tags: [website, theme]
created: 2026-08-29
updated: 2026-08-29T11:52:38Z
started_at: 2026-08-29T11:51:05Z
completed_at: 2026-08-29T11:52:38Z
---

# T-MM-7be25985: Add light/dark theme switcher on the website

## Description

Put a light/dark theme control in the website header. First visit (and until the visitor chooses) follow the operating system color scheme.

## Acceptance criteria

- [x] The site header includes a control that switches between light and dark themes on every page that uses the site chrome.
- [x] With no stored preference, the site uses the visitor's OS light/dark setting (`prefers-color-scheme`).
- [x] Choosing light or dark applies immediately and is remembered on later visits.
- [x] Existing dark-mode tokens and brand logos remain in sync with the resolved theme.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T11:51:05Z | prompt | Marco Mendão | Add a light/dark theme switcher at the top of the website; default from OS. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:51:05Z | 2026-08-29T11:52:38Z | Header theme toggle; defaultTheme system; lint and production build. |
