---
id: R-shelve-discarded-work
type: request
title: Shelve discarded work
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MO
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MO
created: 2026-08-29
updated: 2026-08-29T10:53:00Z
forecast: null
tags:
  - plugin
  - commands
  - dashboard
  - status
aliases:
  - E-MO-0b24529a
source_meetings: []
links: []
---

# Shelve discarded work

## Goal

Let people discard planned work that will never be implemented: `/tkmd-shelf` closes a task, story, or epic as **shelved** (complete but not done), the board shows that distinction, and hide-completed treats shelved items as already finished.

## Scope

- New user command `/tkmd-shelf` alongside init, plan, do, and commit.
- Leaf `status: shelved` for discarded, never-implemented work. Parent status stays a read-time rollup.
- Board lists, Overall tree, and detail chrome distinguish shelved from done.
- Hide-completed (and equivalent completeness filters) hide shelved items the same way they hide done/cancelled.

## Done when

_To be written._

## Out of scope

- Reopening or unshelving via a dedicated command.
- Using `cancelled` as the only shelf representation without a distinct `shelved` status.
- Changing `/tkmd-commit` or making `/tkmd-shelf` commit.

## Open questions

_None yet._
