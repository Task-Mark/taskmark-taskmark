---
id: T-MM-88e93646
type: task
title: Add the Reports tab with a report picker
status: done
priority: high
size: M
points: 5
parent: S-MM-1318bfdd
epic: E-MM-5a80f20a
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
tags: [frontend, reports, ui]
created: 2026-08-31
updated: 2026-08-31T10:55:41Z
started_at: 2026-08-31T07:04:00Z
completed_at: 2026-08-31T07:09:31Z
---

# T-MM-88e93646: Add the Reports tab with a report picker

## Description

Add a `reports` list view alongside `overall`, `workitems`, and `changelog`, shown only when at least one report exists. Build a Reports panel in the same card shape as the changelog panel, with a select listing report dates newest first and the chosen report rendered through the shared markdown component. Selection is local component state so the panel behaves the same in the static export. Wire the tab into both the live board screen and the static board app.

## Acceptance criteria

- [x] A Reports tab appears in the board tab strip when reports exist and is absent otherwise
- [x] The dropdown lists every report, newest first, and defaults to the newest
- [x] Choosing a report renders that report's markdown in place
- [x] `?view=reports` with no reports falls back to the default list view
- [x] The live board and the static export show the same tab and panel behaviour

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T06:47:12Z | prompt | Marco Mendão | From a Cursor plan: add a Reports tab with a dropdown of all reports that lets me pick one, showing the newest by default. |
| 2026-08-31T06:55:00Z | prompt | Marco Mendão | /tkmd-do E-MM-5a80f20a |
| 2026-08-31T10:44:00Z | feedback | Marco Mendão | The Reports tab does not open. |
| 2026-08-31T10:55:41Z | prompt | Cursor agent | Traced the tab to a board screen that never received the query string: the page handed its unresolved `searchParams` promise to the board component, which resolved to an empty object, so every tab fell back to Overall. Pages now await the query and pass the resolved values down. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-31T07:04:00Z | 2026-08-31T07:08:00Z | Added the reports view mode and panel with a date picker, wired the live and static boards, and verified the tab, default selection, and fallback against a running board. |
| Marco Mendão | 2026-08-31T10:44:00Z | 2026-08-31T10:55:41Z | Fixed the tab never opening: the board pages now await their query parameters and pass the resolved values to the board screen, restoring Reports along with Work items and Changelog on both the root and `/board` routes. |
