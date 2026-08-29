---
id: S-MO-aa5fd1ea
type: story
title: Sizing docs and retired metrics pages
status: backlog
priority: medium
size: S
points: 3
parent: E-MO-4b9b509e
epic: E-MO-4b9b509e
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [docs, sizing]
created: 2026-08-28
updated: 2026-08-28T23:15:25Z
started_at: null
completed_at: null
---

# S-MO-aa5fd1ea: Sizing docs and retired metrics pages

## User story

As a planner, I want sizing docs to use the static XS–XXL map and to be told that velocity, README dashboards, and Last-synced changelogs are not part of the product anymore.

## Acceptance criteria

- [ ] Sizing page uses XS=1, S=3, M=5, L=8, XL=13, XXL=21 with the agreed meanings (XXL not sprint-ready; split preferred).
- [ ] Docs state there is no estimate or owner property and that Actual is the sum of closed leaf Work log intervals (parents roll up in the UI).
- [ ] No live docs page teaches Current Speed, ETA, estimate intensity, or a generated board README changelog.
- [ ] Old `/docs/velocity` and `/docs/readme` URLs still redirect to current pages and do not reintroduce retired concepts as current.
