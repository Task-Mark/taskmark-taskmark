---
id: E-011
type: epic
title: Git identity contributors and avatars
status: done
priority: high
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 33
points_source: rolled_up
estimate_minutes: 515
actual_minutes: 8
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
tags: [identity, git, contributors, frontend, plugin]
created: 2026-07-23
updated: 2026-07-28T07:41:00.094Z
started_at: 2026-07-23T17:28:57Z
completed_at: 2026-07-23T17:36:57Z
actual_ms: 480000
---

# E-011: Git identity contributors and avatars

## Goal

Attribute every work item to the people who report it and who resolve it, using the local git config identity (`user.name` / `user.email`). Persist name, email, and initials; surface initials avatars on epic/story/task lists with clear hover labels; keep project READMEs updated with contributors; and show authors on Commits, Work log, and Prompt & feedback.

## Scope

- Read current system git config as the source of identity (not browser OAuth).
- Store on each work item: reporters (creators) and resolvers (developers), supporting multiple people per role.
- Deduplicate when the same person both creates and resolves — show one avatar with combined hover copy.
- Initials-only avatars on epic, story, and task/bug lists.
- Upsert contributors into the project README(s).
- Show associated authors on Commits, Work log, and Prompt & feedback sections.

## Out of scope

- GitHub/GitLab OAuth or profile photos.
- Browser-side reading of git config without a local agent/plugin bridge.
- Full user management UI / auth accounts.

## Success metrics

- New and completed work items carry reporter/resolver identity from local git config.
- Lists show initials avatars with correct hover text for create / resolve / both.
- README Contributors stays in sync with identities seen on the board.
- Activity sections (commits, work log, prompt & feedback) name the authors involved.

## Stories

- [S-039: Git identity data model](stories/S-039-git-identity-data-model/story.md)
- [S-040: Capture git user on create and resolve](stories/S-040-capture-git-user-on-create-resolve/story.md)
- [S-041: README contributors](stories/S-041-readme-contributors/story.md)
- [S-042: Initials avatars on work item lists](stories/S-042-list-initials-avatars/story.md)
- [S-043: Authors on activity logs](stories/S-043-authors-on-activity-logs/story.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 7392380 | taskmark-frontend | 2026-07-23T17:50:21Z | Marco Mendão | add git identity avatars on lists and detail |
| ccebc26 | taskmark-cursor | 2026-07-23T17:50:22Z | Marco Mendão | add git identity helpers and contributor skills |
| e6f0170 | taskmark-taskmark | 2026-07-23T17:50:22Z | Marco Mendão | complete e-011 git identity contributors |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
| 1 | Marco Mendão | 2026-07-23T17:28:57Z | 2026-07-23T17:28:57Z | rollup: children hold shared-batch; delivered E-011 git identity contributors and avatars |

