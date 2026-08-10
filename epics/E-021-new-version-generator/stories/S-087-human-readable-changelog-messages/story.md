---
id: S-087
type: story
title: Human-readable changelog messages
status: backlog
priority: high
size: L
size_source: rolled_up
size_basis: [sum:tasks]
points: 7
points_source: rolled_up
estimate_minutes: 85
actual_minutes: 0
estimate_source: suggested
estimate_basis: [sum:tasks]
session_cap_minutes: 480
parent: E-021
epic: E-021
owner: ""
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [release, versioning, changelog, readme, plugin]
created: 2026-07-29
updated: 2026-07-29T11:30:07.936Z
started_at: null
completed_at: null
actual_ms: 0
---

# S-087: Human-readable changelog messages

## User story

As an end user reading the changelog, I want plain-language descriptions of what changed so I understand the release without decoding board IDs or commit shorthand.

## Acceptance criteria

- [ ] Changelog bullets never lead with or rely on work-item codes (T-/B-/S-/E-NNN).
- [ ] Entries describe user-visible or maintainer-relevant outcomes (e.g. “Fix Vercel production deploy for the board UI” instead of “fix B-009 vercel ui production dep”).
- [ ] Conventions for wording are documented for agents writing Development notes.

## Tasks

- [T-272: Strip work-item IDs from changelog entry text](items/T-272-strip-work-item-ids.md)
- [T-273: Rewrite commits and board titles into end-user messages](items/T-273-rewrite-end-user-messages.md)
- [T-274: Document changelog wording conventions](items/T-274-document-changelog-wording.md)

## Prompt & feedback log

| # | When (UTC) | Kind | Author | Summary |
|---|------------|------|--------|---------|
| 1 | 2026-07-29T07:21:00Z | prompt | Marco Mendão | Create epic for new version generator with stories and tasks; versioned README changelog with Development bucket; meaningful messages without work-item codes |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
