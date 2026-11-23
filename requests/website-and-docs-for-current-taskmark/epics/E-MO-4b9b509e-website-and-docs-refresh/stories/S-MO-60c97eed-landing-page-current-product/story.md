---
id: S-MO-60c97eed
type: story
title: Landing page matches the current product
status: backlog
priority: high
size: M
points: 5
parent: E-MO-4b9b509e
epic: E-MO-4b9b509e
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MO"
resolvers: []
blocked: false
cancelled: false
tags: [website, landing]
created: 2026-08-28
updated: 2026-08-28T23:15:25Z
started_at: null
completed_at: null
---

# S-MO-60c97eed: Landing page matches the current product

## User story

As a visitor, I want the landing page to show the four `/tkmd-*` commands, conflict-resistant markdown, and a hierarchical board so I understand Taskmark as it ships today — not the old command set or SaaS-style velocity.

## Acceptance criteria

- [ ] Hero, console demo, and CTAs use `/tkmd-init`, `/tkmd-create`, `/tkmd-do`, and `/tkmd-commit` only.
- [ ] Console demo IDs and outcomes look like current create/do (collision-resistant IDs, implement without commit, explicit commit).
- [ ] Features describe leaf-only writes, static XS–XXL points, Actual from closed work logs, and multi-repo `/tkmd-commit` — not idle/session-cap velocity or generated indexes.
- [ ] Purpose/board visual shows nested epic → story → task without an `in_progress` badge as the product model.
- [ ] Open-source and docs CTAs still resolve; metadata/SEO copy does not mention retired commands.
