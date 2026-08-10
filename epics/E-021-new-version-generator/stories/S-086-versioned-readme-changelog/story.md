---
id: S-086
type: story
title: Versioned README changelog with Development bucket
status: backlog
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 14
points_source: rolled_up
estimate_minutes: 165
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

# S-086: Versioned README changelog with Development bucket

## User story

As a repo visitor, I want the README changelog organized by released versions plus a Development section so I can see what shipped and what is still in flight.

## Acceptance criteria

- [ ] README Changelog replaces the commit SHA table with versioned sections.
- [ ] A Development section accumulates change notes while work is applied.
- [ ] Creating a new version promotes Development contents under that version heading and clears Development.
- [ ] Prior released version sections remain in the README (newest first).
- [ ] Automation hooks keep Development updated during sync/complete-work without manual README edits.

## Tasks

- [T-268: Replace commit-table README changelog with versioned sections](items/T-268-replace-commit-table-changelog.md)
- [T-269: Append ongoing changes under Development](items/T-269-append-development-notes.md)
- [T-270: Promote Development to released version and clear it](items/T-270-promote-development-on-release.md)
- [T-271: Wire Development logging into sync and complete-work](items/T-271-wire-development-logging.md)

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
