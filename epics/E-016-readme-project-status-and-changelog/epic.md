---
id: E-016
type: epic
title: README project status and changelog
status: done
priority: medium
size: null
size_source: rolled_up
size_basis: [sum:children]
points: 19
points_source: rolled_up
estimate_minutes: 5
actual_minutes: 7
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
tags: [readme, metrics, changelog, automation, plugin]
created: 2026-07-27
updated: 2026-08-14T17:50:46.835Z
started_at: 2026-07-27T07:32:04Z
completed_at: 2026-07-27T07:45:28Z
actual_ms: 447000
---
# E-016: README project status and changelog

## Goal

Keep the board repo `README.md` (`taskmark-taskmark/README.md` in this workspace) updated as a lightweight, always-current project dashboard — mirroring what the board UI shows on the Work items tab for open work, plus headline metrics and a commit-driven changelog.

## Scope

- **Open work items list** — regenerate a markdown section listing only open stories, tasks, and bugs (same item types as the Work items tab). Done, cancelled, and blocked items are excluded unless still in-flight per status rules. Include enough columns to be useful at a glance (id, title, type, status, size/points, parent epic/story where applicable).
- **Project metrics** — show the same headline numbers as the board overview:
  - Total work items
  - Complete work items
  - Current speed (90-day weekly points average, consistent with E-015)
- **Changelog** — add a dedicated `## Changelog` section (marker-delimited like Contributors) that records board-repo commits: date, short SHA, author, and commit message summary.
- **Automation** — refresh the README sections when board state changes (e.g. `sync-status`, `complete-work`, `log-commits`, create/complete item skills) and append changelog entries on every commit to the board repo.
- Reuse existing README marker pattern (`<!-- taskmark:…:begin/end -->`) so scripted upserts do not clobber hand-written intro copy.

## Out of scope

- Listing closed/done work items in the README (metrics may count them; the list is open-only).
- Replacing `INDEX.md` or duplicating its full tables.
- Rendering the README inside the Next.js UI (markdown file is for repo visitors and git hosting).
- Changelog entries for product-repo commits (`taskmark-frontend`, `taskmark-cursor`) unless later scoped — initial focus is the board repo.

## Success metrics

- Opening `README.md` on GitHub or locally shows current open work and metrics without running the UI.
- After `sync-status` or completing work, the open-items and metrics sections update without manual edits.
- Every new commit on the board repo adds one changelog row with accurate metadata.
- Existing Contributors block and intro prose remain intact after refreshes.

## Stories

- [S-059: README project metrics section](stories/S-059-readme-project-metrics-section/story.md)
- [S-060: README open work items list](stories/S-060-readme-open-work-items-list/story.md)
- [S-061: README changelog and automation](stories/S-061-readme-changelog-and-automation/story.md)

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|
| 0c7bfa3 | taskmark-cursor | 2026-07-27T07:46:37Z | Marco Mendão | filter changelog housekeeping commits |
| 764379b | taskmark-cursor | 2026-07-27T07:37:20Z | Marco Mendão | add readme dashboard refresh |

## Work log

| Session | Actor | Started (UTC) | Ended (UTC) | Summary |
|---------|-------|---------------|-------------|---------|
P26-07-27T07:36:40Z | Shared-batch: README project status, open work, changelog automation |
