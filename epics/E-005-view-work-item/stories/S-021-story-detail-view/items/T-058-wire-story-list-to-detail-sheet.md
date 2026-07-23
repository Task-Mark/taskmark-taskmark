---
id: T-058
type: task
title: Wire story list open to story detail sheet
status: done
priority: high
size: S
size_source: suggested
size_basis: [calibrated:T-058]
points: 2
points_source: suggested
estimate_minutes: 30
actual_minutes: 0
estimate_source: manual
estimate_basis: [manual:preserve-plan;burst-delivery]
session_cap_minutes: 480
parent: S-021
epic: E-005
owner: ""
blocked: false
cancelled: false
tags: [ui, stories, frontend, sheet]
created: 2026-07-21
updated: 2026-07-23T07:02:15.905Z
started_at: 2026-07-21T23:53:57Z
completed_at: 2026-07-21T23:57:12Z
actual_ms: 12187
---

# T-058: Wire story list open to story detail sheet

## Description

Connect story list open-detail actions to load story full detail and render the story layout inside the shared sheet.

## Acceptance criteria

- [x] Opening a story from the list loads that story’s detail and shows it in the sheet.
- [x] Loading/error states from S-018 appear for story loads.
- [x] Existing story selection for task drill-down still works.

## Notes

Depends on T-048–T-051, T-053, and T-057.

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-21T23:48:59Z | prompt | Create all user stories and tasks for E-005 view work item |
| 2 | 2026-07-21T23:56:38Z | feedback | Implement E-005 detail sheets delivered |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-21T23:53:57Z | 2026-07-21T23:54:09.187Z | Delivered as part of E-005; shared-batch: 12187 of 195000ms by points |
