---
id: R-cloud-board-markdown-sync
type: request
title: Cloud board markdown sync
status: shipped
requested_by:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
owner:
  - name: Marco Mendão
    email: marco.mendao@betacode.tech
    initials: MM
created: 2026-09-02
updated: 2026-09-02T17:54:46Z
forecast: null
tags:
  - cloud
  - sync
  - api
aliases:
  - E-MM-495d489d
source_meetings: []
links: []
---

# Cloud board markdown sync

## Goal

Developers share one project sync token, set it as `TASKMARK_SYNC_TOKEN` locally, and see their markdown board appear on Taskmark Cloud as a live read-only mirror.

## Done when

- [ ] One opaque sync token per cloud project identifies the destination and authorizes local sync.
- [ ] Local instances send changed markdown files plus a BoardSnapshot cache whenever files change.
- [ ] The hosted board is read-only and reuses the same presentational board UI as the local app.
- [ ] Members can copy the token from project Settings; owners can rotate it.

## Out of scope

_Nothing yet._

## Open questions

_None yet._
