---
id: E-013
type: epic
title: Table sort functionalities
status: backlog
priority: medium
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 0
points_source: rolled_up
estimate_minutes: 0
actual_minutes: 0
estimate_source: rolled_up
estimate_basis: [sum:children]
session_cap_minutes: 480
parent: null
epic: null
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [dashboard, frontend, lists, sort]
created: 2026-07-24
updated: 2026-07-24T17:14:20.339Z
started_at: null
completed_at: null
actual_ms: 0
---

# E-013: Table sort functionalities

## Goal

Let users sort work-item tables by epic, size, title, and id so they can quickly reorder lists to find and compare items.

## Scope

- Sortable columns (or equivalent controls) for: **epic**, **size**, **title**, and **id**.
- Apply across board list tables where those columns appear (Overall drill-down and Work items / list views as applicable).
- Ascending and descending toggle; clear visual indicator of active sort column and direction.
- Compose with existing search, filters, timeframe, and pagination (reset page on sort change when needed).

## Out of scope

- Multi-column / secondary sort keys.
- Persisting sort in the URL or user preferences (optional later).
- Server-side sort APIs.

## Success metrics

- User can sort any supported table by epic, size, title, or id in either direction.
- Active sort is obvious; clearing or switching columns behaves predictably with filters and pagination.

## Stories

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
