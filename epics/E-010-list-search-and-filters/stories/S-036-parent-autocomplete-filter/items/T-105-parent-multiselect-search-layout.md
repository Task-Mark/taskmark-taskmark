---
id: T-105
type: task
title: Parent filter multiselect and search chips layout
status: done
priority: high
size: S
size_source: suggested
size_basis: [T-101, T-102]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 2
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-036
epic: E-010
owner: ""
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
tags: [dashboard, frontend, filters, workitems]
created: 2026-07-23
updated: 2026-07-28T09:08:49.505Z
started_at: 2026-07-23T16:12:45Z
completed_at: 2026-07-23T16:14:55Z
actual_ms: 130000
---
# T-105: Parent filter multiselect and search chips layout

## Description

Make the Work items parent epic/story picker multiselect (match any selected parent), and restyle the list search input to use the same chips-field layout as the tags/parent multiselect pickers.

## Acceptance criteria

- [x] Parent epic/story filter allows selecting multiple parents; empty selection = no parent filter; rows match **any** selected epic or story.
- [x] Parent picker uses the same ComboboxChips input layout as the tags filter.
- [x] List search input uses the same bordered chips-field shell (min-height, padding, border-2, focus ring) as the multiselect pickers.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T16:12:45Z | prompt | Marco Mendão | epic/story picker multiselect; search same layout as multiselect |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T16:12:45Z | 2026-07-23T16:14:55Z | Delivered parent multiselect + search chips layout |
