---
id: S-085
type: story
title: Multi-project version bump
status: backlog
priority: high
size: XL
size_source: rolled_up
size_basis: [sum:tasks]
points: 13
points_source: rolled_up
estimate_minutes: 155
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

# S-085: Multi-project version bump

## User story

As a maintainer, I want to bump versions across linked Taskmark projects with an explicit version or an auto-suggested semver so releases stay consistent without hand-editing every package.json.

## Acceptance criteria

- [ ] Linked projects from REPOS.md (with package versions) are discovered and current versions reported.
- [ ] User can supply an explicit target version.
- [ ] If no version is supplied, the system suggests a semver bump from changes since the last release.
- [ ] Chosen version is written into the relevant project package manifests.
- [ ] A create-version (or equivalent) skill/command orchestrates the bump.

## Tasks

- [T-264: Discover current versions across linked projects](items/T-264-discover-project-versions.md)
- [T-265: Suggest semver bump from changes since last release](items/T-265-suggest-semver-from-changes.md)
- [T-266: Apply user or suggested version to packages](items/T-266-apply-version-to-packages.md)
- [T-267: Add create-version skill and command](items/T-267-create-version-skill.md)

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
