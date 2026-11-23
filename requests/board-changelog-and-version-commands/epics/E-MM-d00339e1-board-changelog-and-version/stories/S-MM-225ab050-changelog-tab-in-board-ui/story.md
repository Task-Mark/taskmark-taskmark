---
id: S-MM-225ab050
type: story
title: Changelog tab in the board UI
status: backlog
priority: high
size: null
points: null
parent: E-MM-d00339e1
epic: E-MM-d00339e1
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [frontend, changelog, ui]
created: 2026-08-29
updated: 2026-08-29T17:33:19Z
started_at: null
completed_at: null
---

# S-MM-225ab050: Changelog tab in the board UI

## User story

As someone using the local board UI, I want a Changelog tab that shows the board-root `CHANGELOG.md` so I can read what shipped without leaving the app — and I do not want that tab at all when the file is missing.

## Acceptance criteria

- [ ] The board UI has a Changelog tab that renders board-root `CHANGELOG.md` (Keep a Changelog markdown)
- [ ] The tab is absent when the file is missing or empty (whitespace-only)
- [ ] Live `taskmark serve`/`dev` and static snapshot builds both honour presence vs absence
- [ ] `?view=changelog` without a changelog falls back to the default list view; the tab is not a README changelog
