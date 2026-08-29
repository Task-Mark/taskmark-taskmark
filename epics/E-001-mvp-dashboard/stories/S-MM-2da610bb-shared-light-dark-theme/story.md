---
id: S-MM-2da610bb
type: story
title: Shared light/dark theme across website and board
status: backlog
priority: medium
size: null
points: null
parent: E-001
epic: E-001
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [theme, website, frontend, cookie]
created: 2026-08-29
updated: 2026-08-29T18:48:30Z
started_at: null
completed_at: null
---

# S-MM-2da610bb: Shared light/dark theme across website and board

## User story

As a visitor, I want to pick light or dark on the website or the board and have that choice follow me on the other, defaulting to my operating system until I choose, so the two surfaces look the same without setting the theme twice.

## Acceptance criteria

- [ ] The website header and the board app bar each include a control that switches between light and dark.
- [ ] With no stored preference, both apps follow the operating system color scheme (`prefers-color-scheme`).
- [ ] Choosing light or dark applies immediately and is stored in a cookie that later visits on that app restore.
- [ ] The same cookie is used by the website and the board so a change on one is used by the other (including `taskmark.dev` and `board.taskmark.dev` via a parent-domain cookie).
