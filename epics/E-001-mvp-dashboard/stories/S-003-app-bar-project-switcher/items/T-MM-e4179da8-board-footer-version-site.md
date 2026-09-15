---
id: T-MM-e4179da8
type: task
title: Show product version and official site in the board footer
status: done
priority: medium
size: S
points: 3
parent: S-003
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
tags: [ui, footer, branding]
created: 2026-09-15
updated: 2026-09-15T17:18:00Z
started_at: 2026-09-15T17:11:32Z
completed_at: 2026-09-15T17:18:00Z
---
# T-MM-e4179da8: Show product version and official site in the board footer

## Description

Add a compact footer to the Taskmark board interface (local UI and Cloud) that shows the current product SemVer and a link to the official website.

## User story

As a user, I want to see which Taskmark version I am running and reach the official site from the board footer so I can check docs and confirm I am on a current release.

## Acceptance criteria

- [x] The board UI footer shows the current product version.
- [x] The footer links to the official Taskmark website (`https://taskmark.dev`).
- [x] The same footer appears on the local board app and Taskmark Cloud.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T17:11:32Z | prompt | Marco Mendão | Show the current product version and a reference to the official site in the Taskmark interface footer. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T17:11:32Z | 2026-09-15T17:18:00Z | Added AppFooter with product SemVer and taskmark.dev; wired it into the local board and Cloud root layouts. |
