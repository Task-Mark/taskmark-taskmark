---
id: R-table-sort-functionalities
type: request
title: Table sort functionalities
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-24
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - dashboard
  - frontend
  - lists
  - sort
aliases:
  - E-013
source_meetings: []
links: []
---

# Table sort functionalities

## Goal

Let users sort work-item tables by epic, size, title, and id so they can quickly reorder lists to find and compare items.

## Scope

- Sortable columns (or equivalent controls) for: **epic**, **size**, **title**, and **id**.
- Apply across board list tables where those columns appear (Overall drill-down and Work items / list views as applicable).
- Ascending and descending toggle; clear visual indicator of active sort column and direction.
- Compose with existing search, filters, timeframe, and pagination (reset page on sort change when needed).

## Done when

- User can sort any supported table by epic, size, title, or id in either direction.
- Active sort is obvious; clearing or switching columns behaves predictably with filters and pagination.

## Out of scope

- Multi-column / secondary sort keys.
- Persisting sort in the URL or user preferences (optional later).
- Server-side sort APIs.

## Open questions

_None yet._
