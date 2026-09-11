---
id: B-MM-6c855151
type: bug
title: Keep one preview and one full presence summary per person
status: done
priority: high
size: S
points: 3
parent: S-MM-f998c021
epic: E-MM-495d489d
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
tags: [cloud, presence, bug]
created: 2026-09-11
updated: 2026-09-11T18:59:04Z
started_at: 2026-09-11T18:51:00Z
completed_at: 2026-09-11T18:59:04Z
---
# B-MM-6c855151: Keep one preview and one full presence summary per person

## Description

Cloud presence can show more than one summary card for the same person, and the card body is not a distinct preview of a longer complete summary. Each contributor must have exactly one presence card. That card shows a short preview sentence. Opening it shows the unrestricted complete summary in the modal.

## Fix criteria

- [x] The presence feed never renders more than one card for the same actor at a time; a newer summary replaces that person.
- [x] The API stores and returns at most one presence record per actor.
- [x] The card body is a simple preview sentence; the modal shows the complete summary, not a duplicate of the preview.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-11T18:52:31Z | prompt | Marco Mendão | A person may only have one summary at a time, with a simple preview on the card and the complete summary in the modal. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-11T18:51:00Z | 2026-09-11T18:59:04Z | Deduped presence cards per actor and stored a short card preview separately from the complete modal summary. |
