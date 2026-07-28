---
id: S-058
type: story
title: Reimplement velocity and time estimates
status: done
priority: low
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 13
points_source: rolled_up
estimate_minutes: 180
actual_minutes: 3
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-015
epic: E-015
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
tags: [plugin, velocity, estimation, future]
created: 2026-07-27
updated: 2026-07-28T14:32:06.722Z
started_at: 2026-07-27T07:19:27Z
completed_at: 2026-07-27T07:23:21Z
actual_ms: 180000
---
# S-058: Reimplement velocity and time estimates

## User story

As a Taskmark user, I want a redesigned speed and estimation system, so project ETAs and create-time estimates match the new Current Speed rules (and whatever replaces the removed 30-day VELOCITY mechanism).

## Acceptance criteria

- [x] Design replaces removed 30-day median min/point estimation (S-057).
- [x] Aligns with E-015 Current Speed (90-day weekly points average) or an explicitly chosen successor rule.
- [x] Restores `VELOCITY.md` / ETA reporting (or a successor board file) as a first-class, documented mechanism.
- [x] Create skills and `recompute-actuals` use the new rules for suggested estimates.

## Tasks

- [T-184: Port Current Speed into recompute and VELOCITY.md](items/T-184-port-current-speed-into-recompute-and-velocity.md)
- [T-185: Suggest estimates from 90-day speed window](items/T-185-suggest-estimates-from-90-day-speed-window.md)
- [T-186: Restore velocity skill command and docs](items/T-186-restore-velocity-skill-command-and-docs.md)
- [T-187: Deploy plugin and seed board VELOCITY.md](items/T-187-deploy-plugin-and-seed-board-velocity.md)


## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T06:10:25Z | prompt | Marco Mendão | Shelf velocity now; track future reimplementation |
| 2 | 2026-07-27T07:19:27Z | prompt | Marco Mendão | Implement remaining incomplete E-015 work items (S-058) |
| 3 | 2026-07-27T07:23:21Z | feedback | Marco Mendão | Delivered S-058 velocity redesign aligned with Current Speed |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 21253c0 | taskmark-cursor | 2026-07-27T07:30:51Z | Marco Mendão | restore velocity with current speed |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
P26-07-27T07:23:21Z | Shared-batch: reimplemented velocity aligned with Current Speed (T-184–T-187) |
