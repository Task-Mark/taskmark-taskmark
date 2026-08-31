# Taskmark

Taskmark is conflict-resistant markdown product memory plus a local board UI.
Work lives as epic, story, task, and bug files. Parent status, points, people,
dates, and logs are derived in the UI from descendant leaves — not generated
dashboard markdown.

This file is static project documentation written by `/tkmd-init`. It is not
a generated dashboard: there is no Last synced metric, Current speed, or
open-work list. Release notes live in `CHANGELOG.md`, written only by
`/tkmd-changelog` and `/tkmd-version`.

## Product repositories

| Repository | Role |
|------------|------|
| taskmark-taskmark | This board (`epics/` and UI stubs) |
| taskmark-cursor | Cursor plugin (commands, skills, rules) |
| taskmark-frontend | Board UI package (`@taskmark/ui`) |
| taskmark-website | Public website and docs |

This repository is the dedicated sibling board (`epics/` at the root). Product
memory is not copied into the other repositories.

## Run the board locally

From this repository:

```bash
npm install
npx taskmark serve
```

The UI listens on [http://localhost:8275](http://localhost:8275).

Live reload while editing board markdown:

```bash
npx taskmark dev
```

`npx taskmark` (the `taskmark` **bin**) works only after a local `@taskmark/ui`
install. Do not run `npx taskmark` in a folder that has not installed that
package — npm may fetch an unrelated `taskmark` package.

## Production build

```bash
npm run build
```

Static HTML and assets are written to `out/`. Preview that export locally:

```bash
npm run preview
```

## Vercel

The board `vercel.json` uses a static `out/` flow (`framework` unset,
`buildCommand`: `npm run build`, `outputDirectory`: `out`). Import this
repository in Vercel and deploy. `@taskmark/ui` must be a production
`dependencies` entry so the install includes the CLI that emits `out/`.

## Docker

This repository includes `Dockerfile` and `compose.yaml`:

```bash
docker compose up --build
```

Then open [http://localhost:8275](http://localhost:8275). The image runs
`npm run build` and serves `out/` with `taskmark preview`.

## Standalone `@taskmark/ui`

When there is **no** local `@taskmark/ui` install, use the published package
name:

```bash
npx @taskmark/ui
```

That starts **workspace** mode: setup wizard and project picker. Inside this
board folder after `npm install`, `npx taskmark serve` (or `npx taskmark`)
binds this board. `npx taskmark open` (or `--workspace`) forces the picker even
when a board is nearby.

## Commands

Use the Cursor plugin in a product workspace:

| Command | Purpose |
|---------|---------|
| `/tkmd-init` | Create board storage, UI stubs, and this static README |
| `/tkmd-plan` | Plan the smallest useful hierarchy from prose |
| `/tkmd-save` | Turn a Cursor Plan mode plan into board items |
| `/tkmd-plan-do` | Plan from prose, then implement only the new items |
| `/tkmd-do` | Implement a target without committing |
| `/tkmd-shelf` | Discard never-implemented work as shelved |
| `/tkmd-changelog` | Rebuild CHANGELOG Unreleased from recent done work |
| `/tkmd-version` | Promote Unreleased and set that SemVer on every linked product |
| `/tkmd-commit` | Commit dirty linked repositories |

This board does not generate `INDEX.md`, `SIZING.md`, or `VELOCITY.md`.
`REPOS.md` is generated locally and gitignored.

Sizing is static: XS=1, S=3, M=5, L=8, XL=13, XXL=21. There is no estimate or
owner property. Actual comes from closed Work log intervals on task/bug leaves.
