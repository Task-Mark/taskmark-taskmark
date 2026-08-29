---
id: T-MM-7786ed4d
type: task
title: Link the website to the live product board
status: done
priority: medium
size: S
points: 3
parent: S-MO-60c97eed
epic: E-MO-4b9b509e
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
tags: [website, landing, demo]
created: 2026-08-29
updated: 2026-08-29T18:40:35Z
started_at: 2026-08-29T18:30:00Z
completed_at: 2026-08-29T18:32:00Z
---

# T-MM-7786ed4d: Link the website to the live product board

## Description

Add a clear link on the public website to https://board.taskmark.dev/ so visitors can open the Taskmark board the team uses to develop Taskmark. That hosted board is also the live demo and proof of concept of the product UI.

## Acceptance criteria

- [x] The website chrome (header and/or primary landing CTAs) includes a control that opens https://board.taskmark.dev/.
- [x] Copy makes it obvious this is the team's real product board and a live demo of Taskmark, not a mock screenshot.
- [x] The link works from the landing page and from other pages that share the site header.
- [x] Existing Start now, docs, and GitHub CTAs still resolve.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T18:20:21Z | prompt | Marco Mendão | Add a website link to https://board.taskmark.dev/ so users can see the team's Taskmark board; also a live demo / proof of concept. |
| 2026-08-29T18:30:00Z | prompt | Marco Mendão | /tkmd-do S-MO-60c97eed |
| 2026-08-29T18:39:00Z | feedback | Marco Mendão | Live product board should be a landing section (Taskmark built with Taskmark; board as an example); remove the hero button. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T18:30:00Z | 2026-08-29T18:32:00Z | Header, hero, and footer links to the live product board. |
| Marco Mendão | 2026-08-29T18:39:00Z | 2026-08-29T18:40:35Z | Replaced the hero CTA with a Built with Taskmark section; header/footer jump to it. |
