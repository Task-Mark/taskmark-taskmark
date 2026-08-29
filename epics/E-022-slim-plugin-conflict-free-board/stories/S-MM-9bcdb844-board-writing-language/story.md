---
id: S-MM-9bcdb844
type: story
title: Board writing language chosen at init
status: backlog
priority: high
size: null
points: null
parent: E-022
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, init, i18n, conventions]
created: 2026-08-29
updated: 2026-08-29T17:29:52Z
started_at: null
completed_at: null
---

# S-MM-9bcdb844: Board writing language chosen at init

## User story

As someone running `/tkmd-init`, I want to choose any writing language for this board (defaulting to the language I usually use with the Cursor agent) so that work items, changelog, README, and other agent-written markdown stay in that language even when I chat in another one.

## Acceptance criteria

- [ ] `/tkmd-init` lets the user pick any language, or records the Cursor-agent default when they do not pick one
- [ ] The chosen language is stored on the board and reused by later `/tkmd-*` sessions
- [ ] Agents write work-item markdown, changelog, README, and other board markdown in that stored language regardless of the chat language
- [ ] Changelog Keep a Changelog headings follow the stored language instead of being hardcoded Portuguese
