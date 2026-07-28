---
id: E-018
type: epic
title: Taskmark website landing page
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 38
points_source: rolled_up
estimate_minutes: 530
actual_minutes: 5
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
resolvers:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
blocked: false
cancelled: false
tags: [website, landing, marketing, frontend]
created: 2026-07-28
updated: 2026-07-28T08:37:10.649Z
started_at: 2026-07-28T07:17:59Z
completed_at: 2026-07-28T07:23:05Z
actual_ms: 306383
---

# E-018: Taskmark website landing page

## Goal

Ship a marketing landing page on `taskmark-website` that explains Taskmark, shows its features, and converts visitors via Start now, docs, contact, and contributor paths. Builds on the E-017 Next.js base.

## Scope

- Hero with Start now CTA and animated console typing of Taskmark commands
- Purpose and motivation
- Features sections covering product capabilities
- Open-source project positioning (built for Cursor at the moment)
- Contact form
- Documentation call to action
- Become a contributor section linking to GitHub

## Out of scope

- Full documentation site content (link/CTA only; docs body may be separate)
- Multi-language localization
- IDE support beyond Cursor messaging
- Paid plans / billing UI

## Success metrics

- Landing page sections above are live and linked
- Start now, docs, and GitHub CTAs resolve correctly
- Contact form accepts and confirms submissions
- Page loads cleanly on desktop and mobile

## Stories

- [S-065: Landing hero with console demo and Start now CTA](stories/S-065-hero-console-demo-start-cta/story.md)
- [S-066: Purpose and motivation section](stories/S-066-purpose-and-motivation/story.md)
- [S-067: Features showcase sections](stories/S-067-features-showcase/story.md)
- [S-068: Open source and Cursor positioning](stories/S-068-opensource-cursor-positioning/story.md)
- [S-069: Contact form](stories/S-069-contact-form/story.md)
- [S-070: Documentation call to action](stories/S-070-documentation-cta/story.md)
- [S-071: Become a contributor section](stories/S-071-become-a-contributor/story.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-28T07:17:59Z | prompt | Marco Mendão | Implement this task E-018 |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 9ce152e | taskmark-website | 2026-07-28T07:33:14Z | Marco Mendão | ship website landing page |
| d8fd130 | taskmark-taskmark | 2026-07-28T07:33:27Z | Marco Mendão | sync taskmark board |
| 62c5488 | taskmark-taskmark | 2026-07-28T07:33:42Z | Marco Mendão | log e-018 commits |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-28T07:17:59Z | 2026-07-28T07:17:59Z | shared-batch rollup: leaves hold billable minutes for landing page delivery |

