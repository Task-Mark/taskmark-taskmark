---
id: T-086
type: task
title: Render markdown in work item detail sheet sections
status: done
priority: high
size: M
size_source: suggested
size_basis: [T-055, T-059]
points: 3
points_source: suggested
estimate_minutes: 5
actual_minutes: 3
estimate_source: suggested
estimate_basis: [calibrated:T-086]
session_cap_minutes: 480
parent: E-005
epic: E-005
owner: ""
blocked: false
cancelled: false
tags: [dashboard, frontend, detail, sheet, markdown]
created: 2026-07-23
updated: 2026-07-23T09:36:52.298Z
started_at: 2026-07-23T09:33:08Z
completed_at: 2026-07-23T09:36:18Z
actual_ms: 190000
---

# T-086: Render markdown in work item detail sheet sections

## Description

Interpret markdown in detail sheet prose sections (goal, scope, user story, description, repro steps, notes, etc.) so headings, lists, links, code, emphasis, and other markdown rules display as formatted content instead of raw text.

## Acceptance criteria

- [x] Epic Goal / Scope / Out of scope / Success metrics render as markdown.
- [x] Story User story (and AC raw fallback) render as markdown.
- [x] Task/bug Description, Repro steps, Notes (and AC/fix criteria raw fallback) render as markdown.
- [x] Common markdown (headings, bold/italic, lists, links, code, blockquotes) is formatted correctly in the sheet.

## Prompt & feedback log

| # | When (UTC) | Kind | Summary |
|---|------------|------|---------|
| 1 | 2026-07-23T09:33:08Z | prompt | Interpret markdown in detail sheet description, repro steps, etc. |

## Commits

| SHA | Repo | Date (UTC) | Message |
|-----|------|------------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | agent | 2026-07-23T09:33:08Z | 2026-07-23T09:36:18Z | react-markdown + GFM for detail sheet prose |
