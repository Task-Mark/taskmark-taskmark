---
id: T-MM-83b18d7d
type: task
title: Changelog and version headings follow board language
status: backlog
priority: high
size: S
points: 3
parent: S-MM-9bcdb844
epic: E-022
reporters:
  - name: "Marco Mendão"
    email: "marco.mendao@betacode.tech"
    initials: "MM"
resolvers: []
blocked: false
cancelled: false
tags: [plugin, changelog, i18n]
created: 2026-08-29
updated: 2026-08-29T17:29:52Z
started_at: null
completed_at: null
---

# T-MM-83b18d7d: Changelog and version headings follow board language

## Description

`/tkmd-changelog` and `/tkmd-version` currently hardcode Portuguese Keep a Changelog headings (`Não publicado`, `Adicionado`, …). Change those skills and the conventions changelog-wording section so Unreleased/category headings and new bullets use the board writing language. Preserve existing dated release sections. Do not write changelog into a README.

## Acceptance criteria

- [ ] Changelog and version skills read the stored board language and write Unreleased, category headings, intro, and new bullets in that language
- [ ] Conventions no longer require Portuguese-only changelog headings; they require Keep a Changelog structure in the board language
- [ ] Existing `## x.y.z - YYYY-MM-DD` sections are left intact when rebuilding Unreleased
- [ ] Commands still write only board-root `CHANGELOG.md` (and version still the board `package.json` version) and never commit

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T17:29:52Z | prompt | Marco Mendão | `/tkmd-init` should let the user choose any project writing language (default: usual Cursor-agent language); work items, changelog, and README must always be written in that language even when chat is in another. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
