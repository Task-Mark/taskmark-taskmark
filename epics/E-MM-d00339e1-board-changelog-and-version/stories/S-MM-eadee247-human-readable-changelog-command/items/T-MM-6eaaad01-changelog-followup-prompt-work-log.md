---
id: T-MM-6eaaad01
type: task
title: Include post-release prompt and work-log follow-ups in Unreleased
status: done
priority: high
size: S
points: 3
parent: S-MM-eadee247
epic: E-MM-d00339e1
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
tags: [plugin, changelog]
created: 2026-09-02
updated: 2026-09-02T21:46:26Z
started_at: 2026-09-02T21:46:26Z
completed_at: 2026-09-02T21:50:00Z
---

# T-MM-6eaaad01: Include post-release prompt and work-log follow-ups in Unreleased

## Description

`/tkmd-changelog` currently qualifies leaves only by `completed_at` (fallback `updated`) after the newest dated release. Follow-up product work logged as Prompt & feedback or Work log on already-done leaves is skipped. Change the collection rules so those post-cutoff rows become Unreleased bullets without restating the original shipped title when the leaf was completed on or before the cutoff.

## User story

As a maintainer, I want Unreleased to include user-visible follow-up work recorded on done leaves after the last release so polish logged on existing tasks is not invisible.

## Acceptance criteria

- [x] A done task/bug qualifies when `completed_at` (fallback `updated`) is after cutoff, or a Prompt & feedback `prompt`/`feedback` timestamp is after cutoff, or a Work log Ended (UTC) is after cutoff
- [x] Follow-ups on leaves completed on or before cutoff are phrased from Work log summaries first, then prompt/feedback paraphrase — not from the original title
- [x] Outcomes already present in a released CHANGELOG section are not repeated in Unreleased
- [x] Conventions, changelog skill, version collection note, and plugin README match this rule
- [x] The skill still never edits item markdown, commits, or pushes

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-02T21:46:26Z | prompt | Marco Mendão | Apply the plan so `/tkmd-changelog` treats Prompt & feedback and Work log rows after the last release as Unreleased changes, by updating the Cursor plugin. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-02T21:46:26Z | 2026-09-02T21:50:00Z | Changelog collection includes post-cutoff prompt, feedback, and work-log rows on done leaves; follow-up wording prefers work-log summaries and skips outcomes already in a dated release. |
