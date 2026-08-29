---
id: T-MM-7b83cead
type: task
title: Show Changelog tab only when changelog exists
status: backlog
priority: high
size: M
points: 5
parent: S-MM-225ab050
epic: E-MM-d00339e1
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, changelog, ui]
created: 2026-08-29
updated: 2026-08-29T17:33:19Z
started_at: null
completed_at: null
---

# T-MM-7b83cead: Show Changelog tab only when changelog exists

## Description

Add a Changelog view next to Overall and Work items. Render the loaded `CHANGELOG.md` with the existing markdown component. Show the tab only when changelog content is present. If `view=changelog` is in the URL but the file is absent, fall back to Overall. Do not add a Changelog tab on boards without a changelog.

## Acceptance criteria

- [ ] List switcher includes Changelog only when changelog content is present
- [ ] Selecting the tab shows the rendered Keep a Changelog markdown (headings, lists, categories)
- [ ] Without a changelog, the tab is not in the switcher and `?view=changelog` opens the default Overall view
- [ ] Live and static board UIs share this behaviour

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:33:19Z | prompt | Marco Mendão | Add a frontend tab for the project changelog; if the changelog does not exist, the tab must not exist either. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
