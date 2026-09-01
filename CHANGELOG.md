# Changelog

All notable changes to this product are recorded in this file.

The format follows Keep a Changelog, and versions follow SemVer.

## Unreleased

## 0.5.0 - 2026-09-01

### Changed

- On small screens, Overall tree rows now show the work-item title first and the remaining details on a second line, without sideways scrolling.
- On small screens, the Work items list now uses stacked rows with the title first, a wrapping metadata line, and a compact sort control instead of a sideways-scrolling table.
- On small screens, Prompt & feedback, Commits, Work log, and other tables in the work-item detail sheet now appear as labelled cards instead of tables.

## 0.4.1 - 2026-08-31

### Fixed

- `taskmark dev` on a board with the UI installed as a package now compiles instead of failing on TypeScript syntax.
- Starting the board when the listen port is already in use now names the port and how to pick another, instead of printing a raw error.

## 0.4.0 - 2026-08-31

### Added

- The `/tkmd-reportme` command was added, which writes a personal, gitignored report of work you finished since the last report, and is documented with the other slash commands.
- A Reports tab was added on the board, with a dropdown of every local report and the newest one selected first.
- A Velocity metric was added that shows current speed against the highest that same speed has been.

### Changed

- Total and Complete work-item cards were replaced by one Complete work items card that shows total over complete.
- Large numbers on Complete work items, Current week, and Velocity now use compact magnitudes such as 1K and 1M.
- Velocity speed is shown as a whole number.
- On small screens the website header now opens from a hamburger menu instead of wrapping onto a second line.

### Fixed

- Complete work-item counts now treat shelved and cancelled work as complete, so the two numbers match when every countable item is finished.

## 0.3.0 - 2026-08-29

### Added

- The board now has a light or dark control that follows the operating system until a theme is chosen, and that choice is remembered in a cookie shared with the website.
- A contribution-style heatmap of completed story points was added on the Overall view, on both the live and static board.
- A Changelog tab was added in the board UI when `CHANGELOG.md` exists, and is hidden when the file is missing.
- `/tkmd-init` now writes a static project README covering purpose, linked repositories, run, and deploy, without restoring generated dashboards.
- The website now links to the live product board as the working Taskmark demo.

### Changed

- Landing-page features were rewritten as outcome cards for agent memory, team visibility, readable changelogs, and hierarchical boards.

## 0.2.0 - 2026-08-29

### Added

- A setup assistant was added that discovers Taskmark projects in the chosen folder, validates the board, and saves the active project.
- An application bar was added with the Taskmark brand and quick switching between projects.
- Lists of epics, stories, tasks, and bugs were added, read directly from local markdown.
- A detail panel was added for any item, with formatted markdown, readable dates, back navigation, and a direct URL.
- Mermaid diagrams can now be drawn in item detail instead of showing as a code block.
- The Work items view was added, with a single table of all work, epic and story labels, progress bars, and points shown on size hover.
- Pagination, search, column sorting, period filter, epic or story filter, tag filter, and an option to hide completed work were added.
- Tasks and bugs can now live directly on an epic, without an intermediate story.
- Creator and resolver identity was added, with initials avatars in lists and authors on activity logs.
- A metrics panel was added with total and completed item counts and the project contributor list.
- The board now opens with a single command: `npx taskmark serve` inside the board folder, or `npx @taskmark/ui` to choose the project.
- The `/tkmd-init`, `/tkmd-plan`, `/tkmd-save`, `/tkmd-plan-do`, `/tkmd-do`, `/tkmd-shelf`, and `/tkmd-commit` Cursor commands were added, the last being the only one that commits.
- A shelved status was added, to close work that will never be implemented without marking it done, with its own look and hidden together with completed work.
- The `/tkmd-changelog` and `/tkmd-version` commands were added, which write release notes in `CHANGELOG.md` and the version on the board `package.json`, without committing or publishing.
- The Taskmark website was created, with a home page, console demo, features, motivation and contribution sections, a contact form, and a light or dark theme switcher.
- Product documentation was published, covering install, command reference, folder structure, file spec, sizes, and workflows.
- Favicons, share images, and SEO metadata were added on the site and the local board.

### Changed

- The Overall view became an expandable hierarchical tree instead of stacked tables, with incomplete-then-newest sorting, search that keeps parent context, keyboard shortcuts, screen-reader support, and expand state kept for the session.
- The board now lives in `<project>/taskmark/` when there is a single repository, or in a dedicated `<common>-taskmark` repository when there are several, and is no longer copied into each product.
- Sizes became fixed, from XS to XXL, with predictable points, instead of estimates calculated from velocity.
- Actual time is now summed from closed work-log intervals, with no estimate or assigned owner.
- Changes are written only to task or bug files; epic and story status, people, logs, and dates are calculated at read time, which avoids conflicts when several people work at once.
- Work identifiers now include the type and the creator identity, and no longer depend on a shared global counter.

### Removed

- The generated `INDEX.md`, `SIZING.md`, `VELOCITY.md`, and board README files were removed, including the changelog that used to live in that README.
- Velocity, estimate calibration, completion forecasts, and the owner field were removed.
- `REPOS.md` is no longer versioned and is generated locally.
- Plugin commands, scripts, and rules that were no longer used were removed.

### Fixed

- Initial setup no longer fails to discover multi-repo boards stored in a single folder.
- The epic list no longer fails when a board file header is malformed.
- The dedicated board repository no longer creates an unnecessary `taskmark/` folder.
- The logo no longer sticks to the bottom edge of the application bar.
- Epic actual time is no longer inflated when several tasks shared the same work session.
- Detail no longer shows the wrong item when another project had the same identifier.
- The board no longer crashes when opening item detail on certain navigations.
- Tasks and bugs no longer need a story in order to belong to an epic.
- Hiding completed work no longer hides epics that still have open work.
- `npx taskmark` no longer runs an unrelated package and always opens the board.
- The board is served at the root, without redirect loops.
- Static board generation no longer fails because of abbreviated paths, incompatible build config, or stale build files, and no longer emits CSS warnings.
- The Vercel-hosted board no longer fails because the UI was declared as a development dependency.
- Accented names no longer produce wrong identities in work identifiers.
