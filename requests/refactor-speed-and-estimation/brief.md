---
id: R-refactor-speed-and-estimation
type: request
title: Refactor speed and estimation
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-21
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - velocity
  - estimation
  - effort
  - plugin
  - conventions
aliases:
  - E-004
source_meetings: []
links: []
---

# Refactor speed and estimation

## Goal

Refactor how Taskmark measures speed and estimates work: keep AI/human **session effort**, compute **minutes-per-point over a 1-month window**, estimate from that speed, redefine **actual** as wall-clock from start→complete, and add explicit **start/end** actions with parent/child cascade.

## Scope

- Continue recording elapsed session time (work log) as effort spent by AI/human.
- Calculate story-point speed from done tasks/stories/epics in a rolling **1-month** window.
- Derive new-item `estimate_minutes` from that speed × points.
- Recalculate `actual_minutes` from `started_at` → `completed_at` (not calendar idle alone without a start).
- Handle complete-without-start / missing dates explicitly.
- Start action for task/story/epic; starting a task also starts its story and epic if needed.
- End/complete action; ending the last open child closes the parent story/epic.

## Done when

- New estimates use 1-month median min/point when enough samples exist; otherwise seed table.
- Done items with both start and complete timestamps have actual = that span (with documented caps if any).
- Start/end skills cascade correctly; last child complete closes parents.
- Session work-log effort remains available (not discarded).

## Out of scope

- Changing Fibonacci points map or t-shirt labels.
- Dashboard UI charts (plugin/board model first; UI can follow).
- Billing/invoicing integrations.

## Open questions

_None yet._
