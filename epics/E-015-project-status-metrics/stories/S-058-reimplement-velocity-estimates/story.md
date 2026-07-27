---
id: S-058
type: story
title: Reimplement velocity and time estimates
status: backlog
priority: low
size: XL
size_source: suggested
size_basis: []
points: 13
points_source: suggested
estimate_minutes: 180
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:14min/pt]
session_cap_minutes: 480
parent: E-015
epic: E-015
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, velocity, estimation, future]
created: 2026-07-27
updated: 2026-07-27T07:06:27.645Z
started_at: null
completed_at: null
actual_ms: 0
---

# S-058: Reimplement velocity and time estimates

## User story

As a Taskmark user, I want a redesigned speed and estimation system, so project ETAs and create-time estimates match the new Current Speed rules (and whatever replaces the removed 30-day VELOCITY mechanism).

## Acceptance criteria

- [ ] Design replaces removed 30-day median min/point estimation (S-057).
- [ ] Aligns with E-015 Current Speed (90-day weekly points average) or an explicitly chosen successor rule.
- [ ] Restores `VELOCITY.md` / ETA reporting (or a successor board file) as a first-class, documented mechanism.
- [ ] Create skills and `recompute-actuals` use the new rules for suggested estimates.

## Tasks

_(None yet — future work.)_

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-27T06:10:25Z | prompt | Marco Mendão | Shelf velocity now; track future reimplementation |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
