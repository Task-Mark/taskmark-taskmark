---
id: T-111
type: task
title: Define contributor identity schema in conventions
status: done
priority: high
size: XS
size_source: suggested
size_basis: [velocity:similar]
points: 1
points_source: suggested
estimate_minutes: 15
actual_minutes: 0
estimate_source: suggested
estimate_basis: [velocity:30d:16min/pt]
session_cap_minutes: 480
parent: S-039
epic: E-011
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
tags: [identity, conventions, plugin]
created: 2026-07-23
updated: 2026-07-28T08:37:10.649Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 0
---

# T-111: Define contributor identity schema in conventions

## Description

Document the canonical contributor identity object used across board markdown and plugin helpers: `name`, `email`, `initials`, plus how initials are derived from name when not provided.

## Acceptance criteria

- [x] Conventions (or frontmatter ref) define the identity shape and reporters/resolvers roles.
- [x] Initials derivation rules are specified (e.g. first letter of first + last token).
- [x] Multi-author arrays and email-based uniqueness are documented.

## Notes

Browser cannot read git config; identity is always supplied by local plugin/agent.

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-23T17:28:57Z | prompt | Marco Mendão | User asked to start developing epic E-011. |
| 2 | 2026-07-23T17:36:57Z | feedback | Marco Mendão | Delivered identity schema, git helper, README sync, list avatars, activity authors. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T17:28:57Z | 2026-07-23T17:28:57Z | delivered; shared-batch: 0 of 8min by points |
