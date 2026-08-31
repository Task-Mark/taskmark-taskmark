---
id: T-MM-88e93646
type: task
title: Add the Reports tab with a report picker
status: backlog
priority: high
size: M
points: 5
parent: S-MM-1318bfdd
epic: E-MM-5a80f20a
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, reports, ui]
created: 2026-08-31
updated: 2026-08-31T06:47:12Z
started_at: null
completed_at: null
---

# T-MM-88e93646: Add the Reports tab with a report picker

## Description

Add a `reports` list view alongside `overall`, `workitems`, and `changelog`, shown only when at least one report exists. Build a Reports panel in the same card shape as the changelog panel, with a select listing report dates newest first and the chosen report rendered through the shared markdown component. Selection is local component state so the panel behaves the same in the static export. Wire the tab into both the live board screen and the static board app.

## Acceptance criteria

- [ ] A Reports tab appears in the board tab strip when reports exist and is absent otherwise
- [ ] The dropdown lists every report, newest first, and defaults to the newest
- [ ] Choosing a report renders that report's markdown in place
- [ ] `?view=reports` with no reports falls back to the default list view
- [ ] The live board and the static export show the same tab and panel behaviour

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-31T06:47:12Z | prompt | Marco Mendão | From a Cursor plan: add a Reports tab with a dropdown of all reports that lets me pick one, showing the newest by default. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
