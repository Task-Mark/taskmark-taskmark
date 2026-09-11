---
id: T-MM-2500c26f
type: task
title: Render presence cards above the Cloud worklog feed
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
tags: [cloud, ui, presence]
created: 2026-09-03
updated: 2026-09-11T19:02:02Z
started_at: 2026-09-03T21:56:00Z
completed_at: 2026-09-03T22:02:00Z
---
# T-MM-2500c26f: Render presence cards above the Cloud worklog feed

## Description

Add a shared presence feed that Cloud fills from the activity endpoint. Render it on the left, stacked above the pace gauge in one floating column, with the same avatar and bubble chrome as the worklog feed: name in the header, quoted sentence in the body, no item code tag. One card per person; a newer pulse replaces that person. Seed silently on first fetch; play the existing bong when a card is new or its summary changes. Hide on mobile like the worklog feed. Leave the speedometer unchanged.

## Acceptance criteria

- [x] Cloud presence cards sit on the left, above the pace gauge, and reuse Message / avatar / Bubble chrome.
- [x] Presence body is a quoted sentence with no item code tag.
- [x] One card per actor; a later pulse replaces that actor instead of stacking.
- [x] First fetch seeds silently; later new or changed cards play the existing feed sound.
- [x] The feed stays hidden on small screens; the left speedometer is unchanged.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-11T19:02:02Z | prompt | Marco Mendão | Show the avatar and the relative generation time inside the full summary modal. |
| 2026-09-07T18:11:49Z | prompt | Marco Mendão | Show a simple summary of at most 180 characters on each card and open an unrestricted complete summary in a modal when clicked. |
| 2026-09-03T22:06:26Z | feedback | Marco Mendão | The AI summary per person belongs on the left, not on the right. |
| 2026-09-03T21:56:00Z | prompt | Marco Mendão | Cursor plan: render presence cards above the Cloud worklog feed. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-11T18:59:30Z | 2026-09-11T19:02:02Z | Gave the full summary modal a header with the person's avatar, name, and the time the summary was generated. |
| Marco Mendão | 2026-09-07T18:08:00Z | 2026-09-07T18:11:49Z | Stored compact and complete presence summaries, limited cards to 180 characters, and opened the full text in an accessible modal. |
| Marco Mendão | 2026-09-03T22:03:00Z | 2026-09-03T22:06:26Z | Moved the presence summaries into their own left column above the pace gauge. |
| Marco Mendão | 2026-09-03T21:56:00Z | 2026-09-03T22:02:00Z | Rendered quoted presence cards above the Cloud worklog feed. |
