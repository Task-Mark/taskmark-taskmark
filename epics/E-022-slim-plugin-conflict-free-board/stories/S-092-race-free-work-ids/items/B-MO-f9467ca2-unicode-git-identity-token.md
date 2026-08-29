---
id: B-MO-f9467ca2
type: bug
title: ASCII ID identity splits accented git names (MM becomes MO)
status: done
priority: high
size: S
points: 3
parent: S-092
epic: E-022
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
tags: [plugin, identity, ids]
created: 2026-08-29
updated: 2026-08-29T11:16:30Z
started_at: 2026-08-29T11:14:20Z
completed_at: 2026-08-29T11:16:30Z
---

# B-MO-f9467ca2: ASCII ID identity splits accented git names (MM becomes MO)

## Description

`allocate-id.py` builds the identity token with `re.findall(r"[A-Za-z0-9]+", name)`. That pattern is ASCII-only, so a last name like Mendão is split at ã into `Mend` and `o`. First letter of the first token plus first letter of the last token becomes **MO** instead of **MM**.

`git-identity.py` `derive_initials` still splits on whitespace/punctuation only and correctly yields **MM** for `Marco Mendão`. Planning stamps ID identity from the allocator, so new item IDs (and often frontmatter `initials` copied from that token) show MO even though git `user.name` did not change.

This item's own id (`B-MO-f9467ca2`) is an example of the broken token. Do not rewrite historical IDs.

## Fix criteria

- [x] `identity_token("Marco Mendão")` (and equivalent NFC/NFD spellings) is `MM`, not `MO`.
- [x] Identity tokens treat Unicode letters as part of a word; they do not split on diacritics.
- [x] Allocator identity matches `git-identity.py` initials for the same `user.name` (shared helper or the same word-split rules).
- [x] Tests cover accented given/family names; existing ASCII names stay 2–12 uppercase letters/digits.
- [x] Historical `*-MO-*` ids remain valid; no board rewrite.

## Prompt & feedback

| When (UTC) | Kind | Author | Summary |
|------------|------|--------|---------|
| 2026-08-29T11:12:25Z | prompt | Marco Mendão | Git user initials that used to be MM for Marco Mendão are now MO; report the bug and plan a fix. |
| 2026-08-29T11:14:20Z | prompt | Marco Mendão | `/tkmd-do`: implement every backlog work item under epic E-022. |
| 2026-08-29T11:26:00Z | feedback | Marco Mendão | Reported that bug leaves look uncounted because E-022 shows 35/35 and hide-completed hides this bug. Verified counts include bugs; this leaf reads `done` because the E-022 `/tkmd-do` run closed it right after planning. |

## Commits

| SHA | Repo | Date (UTC) | Author | Message |
|-----|------|------------|--------|---------|

## Work log

| Actor | Started (UTC) | Ended (UTC) | Summary |
|-------|---------------|-------------|---------|
| Marco Mendão | 2026-08-29T11:14:20Z | 2026-08-29T11:16:30Z | Folded Unicode letters into identity tokens so Mendão yields MM, shared with git-identity. |
