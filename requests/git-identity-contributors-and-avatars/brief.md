---
id: R-git-identity-contributors-and-avatars
type: request
title: Git identity contributors and avatars
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-23
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - identity
  - git
  - contributors
  - frontend
  - plugin
aliases:
  - E-011
source_meetings: []
links: []
---

# Git identity contributors and avatars

## Goal

Attribute every work item to the people who report it and who resolve it, using the local git config identity (`user.name` / `user.email`). Persist name, email, and initials; surface initials avatars on epic/story/task lists with clear hover labels; keep project READMEs updated with contributors; and show authors on Commits, Work log, and Prompt & feedback.

## Scope

- Read current system git config as the source of identity (not browser OAuth).
- Store on each work item: reporters (creators) and resolvers (developers), supporting multiple people per role.
- Deduplicate when the same person both creates and resolves — show one avatar with combined hover copy.
- Initials-only avatars on epic, story, and task/bug lists.
- Upsert contributors into the project README(s).
- Show associated authors on Commits, Work log, and Prompt & feedback sections.

## Done when

- New and completed work items carry reporter/resolver identity from local git config.
- Lists show initials avatars with correct hover text for create / resolve / both.
- README Contributors stays in sync with identities seen on the board.
- Activity sections (commits, work log, prompt & feedback) name the authors involved.

## Out of scope

- GitHub/GitLab OAuth or profile photos.
- Browser-side reading of git config without a local agent/plugin bridge.
- Full user management UI / auth accounts.

## Open questions

_None yet._
