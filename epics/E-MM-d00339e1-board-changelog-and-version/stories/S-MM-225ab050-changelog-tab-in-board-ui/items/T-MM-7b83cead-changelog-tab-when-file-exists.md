---
id: T-MM-7b83cead
type: task
title: Show Changelog tab only when changelog exists
status: done
priority: high
size: M
points: 5
parent: S-MM-225ab050
epic: E-MM-d00339e1
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
tags: [frontend, changelog, ui]
created: 2026-08-29
updated: 2026-08-29T18:09:45Z
started_at: 2026-08-29T18:05:00Z
completed_at: 2026-08-29T18:09:45Z
---

# T-MM-7b83cead: Show Changelog tab only when changelog exists

## Description

Add a Changelog view next to Overall and Work items. Render the loaded `CHANGELOG.md` with the existing markdown component. Show the tab only when changelog content is present. If `view=changelog` is in the URL but the file is absent, fall back to Overall. Do not add a Changelog tab on boards without a changelog.

## Acceptance criteria

- [x] List switcher includes Changelog only when changelog content is present
- [x] Selecting the tab shows the rendered Keep a Changelog markdown (headings, lists, categories)
- [x] Without a changelog, the tab is not in the switcher and `?view=changelog` opens the default Overall view
- [x] Live and static board UIs share this behaviour

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:33:19Z | prompt | Marco Mendão | Add a frontend tab for the project changelog; if the changelog does not exist, the tab must not exist either. |
| 2026-08-29T18:05:00Z | prompt | Marco Mendão | /tkmd-do S-MM-225ab050 and S-MM-2d3bf631 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T18:07:00Z | 2026-08-29T18:08:15Z | Changelog tab and view=changelog fallback on live and static board UI. |
