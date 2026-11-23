---
id: R-project-status-metrics
type: request
title: Project status metrics
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-27
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - frontend
  - metrics
  - dashboard
  - velocity
  - contributors
aliases:
  - E-015
source_meetings: []
links: []
---

# Project status metrics

## Goal

Show at-a-glance project health on the board: total work items, completed work items, current delivery speed, and a simple contributors view — presented as clean metric cards in the style of the provided neo-brutalism reference (bold value, titled card, accent icon with hard black shadow).

## Scope

- Metric cards for:
  - **Total work items** — count of user stories, bugs, and tasks (exclude epics).
  - **Complete work items** — same types with `status: done`.
  - **Current speed** — average weekly story points completed over a 90-day window anchored at the most recently completed task/bug. Exclude the **current** ISO week and weeks with **0** points; average only the remaining (active) weeks.
- A simple **contributors** view listing people who have reported or resolved work on the project (reuse existing identity / initials avatars).
- Shared card visual language matching the reference: white card, solid black border, large bold value, accent icon square with hard offset shadow.

## Done when

- Selected project board shows Total, Complete, and Current Speed cards with correct live values.
- Current speed matches the 90-day weekly points average rule above.
- Contributors view lists unique project people with initials avatars.
- Layout remains readable on desktop and mobile.

## Out of scope

- Revenue / orders / conversion-style business KPIs from the reference image.
- Per-metric “vs last period” trend pills (nice-to-have later; not required for this epic).
- Editing contributor identity from the metrics UI.
- Legacy 30-day `VELOCITY.md` / time-estimate mechanism **removed** (S-057); optional redesign tracked in S-058.

## Open questions

_None yet._
