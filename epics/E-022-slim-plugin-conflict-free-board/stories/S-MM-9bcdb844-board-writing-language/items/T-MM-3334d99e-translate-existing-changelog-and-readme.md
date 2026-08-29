---
id: T-MM-3334d99e
type: task
title: Translate existing changelog and project README into the board language
status: backlog
priority: high
size: M
points: 5
parent: S-MM-9bcdb844
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [changelog, readme, i18n]
created: 2026-08-29
updated: 2026-08-29T17:31:00Z
started_at: null
completed_at: null
---

# T-MM-3334d99e: Translate existing changelog and project README into the board language

## Description

Rewrite the board-root `CHANGELOG.md` (intro, Unreleased, category headings, and existing dated release bullets) and the static project README owned by init (workspace/product README, not generated dashboards) into the stored board writing language. Keep Keep a Changelog structure, SemVer section titles `## x.y.z - YYYY-MM-DD`, and command/package names. Do not put a changelog in the README. Do not rewrite plugin, frontend, or website READMEs except if they are the init static project README. Future `/tkmd-changelog` heading language is T-MM-83b18d7d; this leaf is the one-time translation of current files.

## Acceptance criteria

- [ ] Board `CHANGELOG.md` intro, Unreleased heading, category headings, and all existing bullets are in the stored writing language
- [ ] Version headings stay `## x.y.z - YYYY-MM-DD`; bullets still omit work-item IDs
- [ ] The static project README prose is in the stored writing language; Last synced / Current speed / README changelog remain absent
- [ ] Plugin/frontend/website READMEs are left unchanged unless they are that same static project README

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:31:00Z | prompt | Marco Mendão | Translate all work items, changelog, and README to the writing language chosen for the Taskmark project. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
