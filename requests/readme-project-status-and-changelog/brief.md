---
id: R-readme-project-status-and-changelog
type: request
title: README project status and changelog
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-07-27
updated: 2026-08-28T12:37:43.783Z
forecast: null
tags:
  - readme
  - metrics
  - changelog
  - automation
  - plugin
aliases:
  - E-016
source_meetings: []
links: []
---

# README project status and changelog

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

## Done when

- Opening `README.md` on GitHub or locally shows current open work and metrics without running the UI.
- After `sync-status` or completing work, the open-items and metrics sections update without manual edits.
- Every new commit on the board repo adds one changelog row with accurate metadata.
- Existing Contributors block and intro prose remain intact after refreshes.

## Out of scope

- Listing closed/done work items in the README (metrics may count them; the list is open-only).
- Replacing `INDEX.md` or duplicating its full tables.
- Rendering the README inside the Next.js UI (markdown file is for repo visitors and git hosting).
- Changelog entries for product-repo commits (`taskmark-frontend`, `taskmark-cursor`) unless later scoped — initial focus is the board repo.

## Open questions

_None yet._
