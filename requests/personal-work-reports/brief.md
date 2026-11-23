---
id: R-personal-work-reports
type: request
title: Personal work reports
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-08-31
updated: 2026-08-31T06:47:12Z
forecast: null
tags:
  - reports
  - plugin
  - frontend
  - changelog
aliases:
  - E-MM-5a80f20a
source_meetings: []
links: []
---

# Personal work reports

## Goal

Let a contributor ask the agent what they personally delivered since their last report, and read it as plain human prose. A new `/tkmd-reportme` command collects the done work resolved by the current git identity and writes a local report file; the board UI gains a Reports tab that lists every report and opens the newest one by default.

## Scope

- Agent command `/tkmd-reportme` in the same style as the existing `/tkmd-*` set
- Report files in a gitignored `.reports/` directory at the board root, one per report, named `report-YYYYMMDD.md`
- Bullets phrased like `CHANGELOG.md`: past tense, user-visible outcomes, no work-item codes, board writing language
- Only the current git identity's done leaves, with the cutoff taken from the previous report's filename date
- A Reports tab in the live board UI and the static snapshot, with a report picker defaulting to the newest report

## Done when

- Running the command twice in a row produces no duplicated bullets across reports
- A contributor can read a report without knowing any work-item ID
- Report files never appear in `git status` on any linked repository
- The Reports tab is absent when no report has been generated yet

## Out of scope

- Changing or replacing `CHANGELOG.md`, which stays team-wide and committed
- Committing, pushing, or publishing reports; they are deliberately local-only
- Reports for other people, per-person filtering in the UI, or exports beyond markdown
- Time tracking, effort totals, or velocity figures inside the report

## Open questions

_None yet._
