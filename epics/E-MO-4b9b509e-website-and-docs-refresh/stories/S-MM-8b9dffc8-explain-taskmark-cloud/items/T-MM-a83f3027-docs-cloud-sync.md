---
id: T-MM-a83f3027
type: task
title: Document how local boards sync to Taskmark Cloud
status: done
priority: high
size: S
points: 3
parent: S-MM-8b9dffc8
epic: E-MO-4b9b509e
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
tags: [website, docs, cloud, sync]
created: 2026-09-15
updated: 2026-09-15T16:52:00Z
started_at: 2026-09-15T16:37:00Z
completed_at: 2026-09-15T16:45:00Z
---
# T-MM-a83f3027: Document how local boards sync to Taskmark Cloud

## Description

Add a `/docs/cloud` page that explains Taskmark Cloud and the current sync path: create a Cloud project, copy the token from Cloud Settings, put `TASKMARK_SYNC_TOKEN` in the board `.config`, then run `taskmark dev` or `taskmark serve`.

## User story

As a developer, I want docs that tell me how to connect my local Taskmark board to Cloud so the team can read the same markdown without extra tooling.

## Acceptance criteria

- [x] `/docs/cloud` explains why Cloud exists and that local markdown remains the source of truth.
- [x] The page lists the sync steps using `.config` (not a local Settings tab).
- [x] Docs overview, sidebar, and suggested path include the Cloud page.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T16:37:00Z | prompt | Marco Mendão | Add website information about Taskmark Cloud: its purpose and how local boards sync with Cloud. |
| 2026-09-15T16:45:00Z | feedback | Marco Mendão | Expand the Cloud docs with a practical configuration guide alongside the complete Cloud marketing page. |
| 2026-09-15T16:51:30Z | prompt | Marco Mendão | Add a New tag on the sidebar Cloud item so users can see that it is new. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T16:37:00Z | 2026-09-15T16:45:00Z | Added /docs/cloud with purpose, .config token steps, and sidebar/overview links. |
| Marco Mendão | 2026-09-15T16:45:00Z | 2026-09-15T16:50:00Z | Expanded Cloud docs with configuration reference, sync verification output, and troubleshooting guidance. |
| Marco Mendão | 2026-09-15T16:51:30Z | 2026-09-15T16:52:00Z | Added a New badge on Cloud in the docs sidebar and site navigation. |
