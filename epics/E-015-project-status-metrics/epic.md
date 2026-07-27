---
id: E-015
type: epic
title: Project status metrics
status: in_progress
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 39
points_source: rolled_up
estimate_minutes: 550
actual_minutes: 9
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
tags: [frontend, metrics, dashboard, velocity, contributors]
created: 2026-07-27
updated: 2026-07-27T07:06:27.645Z
started_at: 2026-07-27T06:10:41Z
completed_at: null
actual_ms: 540000
---
# E-015: Project status metrics

## Goal

Show at-a-glance project health on the board: total work items, completed work items, current delivery speed, and a simple contributors view — presented as clean metric cards in the style of the provided neo-brutalism reference (bold value, titled card, accent icon with hard black shadow).

## Scope

- Metric cards for:
  - **Total work items** — count of user stories, bugs, and tasks (exclude epics).
  - **Complete work items** — same types with `status: done`.
  - **Current speed** — average weekly story points completed over a 90-day window anchored at the most recently completed task/bug. Exclude the **current** ISO week and weeks with **0** points; average only the remaining (active) weeks.
- A simple **contributors** view listing people who have reported or resolved work on the project (reuse existing identity / initials avatars).
- Shared card visual language matching the reference: white card, solid black border, large bold value, accent icon square with hard offset shadow.

## Out of scope

- Revenue / orders / conversion-style business KPIs from the reference image.
- Per-metric “vs last period” trend pills (nice-to-have later; not required for this epic).
- Editing contributor identity from the metrics UI.
- Legacy 30-day `VELOCITY.md` / time-estimate mechanism **removed** (S-057); optional redesign tracked in S-058.

## Success metrics

- Selected project board shows Total, Complete, and Current Speed cards with correct live values.
- Current speed matches the 90-day weekly points average rule above.
- Contributors view lists unique project people with initials avatars.
- Layout remains readable on desktop and mobile.

## Stories

- [S-053: Metrics cards UI shell](stories/S-053-metrics-cards-ui/story.md)
- [S-054: Total and complete work item counts](stories/S-054-work-item-count-metrics/story.md)
- [S-055: Current speed metric](stories/S-055-current-speed-metric/story.md)
- [S-056: Project contributors view](stories/S-056-project-contributors-view/story.md)
- [S-057: Remove legacy velocity and time estimates](stories/S-057-shelf-legacy-velocity/story.md)
- [S-058: Reimplement velocity and time estimates](stories/S-058-reimplement-velocity-estimates/story.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| d5f8f02 | taskmark-frontend | 2026-07-27T07:08:31Z | Marco Mendão | add project metrics and calendar points |
| a494e58 | taskmark-taskmark | 2026-07-27T06:19:46Z | Marco Mendão | add e-015 metrics and remove velocity board |
| 1a8522f | taskmark-frontend | 2026-07-27T06:19:45Z | Marco Mendão | drop est actual columns and velocity timing notes |
| b942bb0 | taskmark-cursor | 2026-07-27T06:19:45Z | Marco Mendão | remove velocity and time-estimate sizing |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-27T06:25:20Z | 2026-07-27T06:25:20Z | Parent rollup: E-015 metrics UI; billable on T-169–T-176 (shared-batch) |
