---
id: T-MM-d70ef3ac
type: task
title: Minimize then hover-expand messages and the worklog count card
status: done
priority: high
size: M
points: 5
parent: S-MM-715f96e0
epic: E-MM-69ccb23d
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
tags: [ui, worklog, presence, speedometer]
created: 2026-09-15
updated: 2026-09-15T23:03:00Z
started_at: 2026-09-15T22:11:00Z
completed_at: 2026-09-15T22:28:00Z
---
# T-MM-d70ef3ac: Minimize then hover-expand messages and the worklog count card

## Description

Add a control that collapses the floating worklog messages, presence summaries, and worklog count card. After minimize, those components stay collapsed until the user hovers them, then expand again for the hover. Local and npx boards should show the same floating chrome as Cloud.

## Acceptance criteria

- [x] A visible control in the app bar minimizes the floating messages and the worklog count card.
- [x] The app bar control uses bookmark on and bookmark off icons.
- [x] After minimize, corner handles sit in the bottom-left and bottom-right with inset from the footer, and hovering a handle or the matching page edge slides the chrome in like a sheet above the handle.
- [x] After minimize, the bottom-left handle shows the pace icon above today's worklog count.
- [x] After minimize, a new worklog appears as a toaster on the right; later messages stack and each disappears after 10 seconds.
- [x] After minimize, a generated presence summary opens that sheet for 10 seconds.
- [x] Leaving hover returns them to the minimized state until the user expands them again with the control or another hover.
- [x] Cloud boards start with messages minimized until the user expands them.
- [x] The expanded or minimized preference is stored in a cookie and survives refresh and later visits.
- [x] Local, npx static, and Cloud boards share this chrome.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-09-15T23:03:00Z | prompt | Marco Mendão | Increase left peek padding and keep top and bottom equal. |
| 2026-09-15T23:00:00Z | prompt | Marco Mendão | Add padding on the left peek so the pace icon is not flush with the top of the button. |
| 2026-09-15T22:58:00Z | prompt | Marco Mendão | Put a smaller pace icon above the worklog count on the bottom-left handle. |
| 2026-09-15T22:50:00Z | prompt | Marco Mendão | Show only the latest worklog as a toaster; stack newer ones and dismiss them after 10 seconds. |
| 2026-09-15T22:41:00Z | prompt | Marco Mendão | Default Cloud messages to minimized and persist the setting in a cookie across refresh and later visits. |
| 2026-09-15T22:37:00Z | prompt | Marco Mendão | While minimized, show each new worklog message and each generated summary for 10 seconds. |
| 2026-09-15T22:34:00Z | prompt | Marco Mendão | Keep worklog messages and the work-item counter off the footer and off their hover buttons, and inset the buttons from the bottom. |
| 2026-09-15T22:32:00Z | prompt | Marco Mendão | Put the hover handles in the bottom corners, animate the chrome like a sheet, and also open it from the left or right page edge. |
| 2026-09-15T22:30:00Z | prompt | Marco Mendão | Put the maximize/minimize control in the app bar and use bookmark on/off icons. |
| 2026-09-15T22:11:00Z | prompt | Marco Mendão | Add a button to minimize the messages and work-item count card; after that they should expand only on hover, on local, npx, and Cloud boards. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-09-15T23:03:00Z | 2026-09-15T23:03:00Z | Matched extra top and bottom padding on the left peek. |
| Marco Mendão | 2026-09-15T23:00:00Z | 2026-09-15T23:00:00Z | Padded the left peek so the pace icon sits off the top edge. |
| Marco Mendão | 2026-09-15T22:58:00Z | 2026-09-15T22:58:00Z | Added a compact pace icon above the count on the left peek. |
| Marco Mendão | 2026-09-15T22:50:00Z | 2026-09-15T22:50:00Z | Showed collapsed worklogs as a 10-second toaster stack instead of opening the full sheet. |
| Marco Mendão | 2026-09-15T22:41:00Z | 2026-09-15T22:41:00Z | Defaulted Cloud chrome to minimized and stored the preference in a one-year cookie. |
| Marco Mendão | 2026-09-15T22:37:00Z | 2026-09-15T22:37:00Z | Pulsed collapsed worklog and summary sheets open for 10 seconds on new items. |
| Marco Mendão | 2026-09-15T22:34:00Z | 2026-09-15T22:34:00Z | Lifted chrome and peek buttons above the footer so sheets sit on the handles. |
| Marco Mendão | 2026-09-15T22:32:00Z | 2026-09-15T22:32:00Z | Opened collapsed chrome from corner handles or page edges with a sheet slide. |
| Marco Mendão | 2026-09-15T22:30:00Z | 2026-09-15T22:30:00Z | Moved the chrome toggle into the app bar with bookmark on/off icons. |
| Marco Mendão | 2026-09-15T22:11:00Z | 2026-09-15T22:28:00Z | Added shared floating chrome with minimize and hover-expand on local, npx, and Cloud boards. |
