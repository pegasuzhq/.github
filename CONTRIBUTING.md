# Contributing

The baseline for every Pegasuz repository. A repository that ships its own
`CONTRIBUTING.md` overrides this one — read that instead.

## Before you start

Read the repository's `AGENTS.md` and `README.md`. Anything specific — how to
run it, which gates must pass, what not to touch — lives there, not here.

## Branches and commits

- Branch from the default branch with the name Linear generates for the issue
  (`user/eng-123-slug`). A branch carries the key or it is not tracker work.
- [Conventional commits](https://www.conventionalcommits.org): `feat:`, `fix:`,
  `docs:`, `chore:`, `refactor:`, `test:`.
- One reason per commit. If the message needs an "and", it is two commits.
- Push your work. Servers deploy from the remote; unpushed work does not exist.

## Issues

Issues live in **Linear** (`linear.app/pegasuz`, team `ENG` for every repository, `SUP` for
tenant tickets). GitHub keeps code and pull requests; its Issues feature is switched off in
every repository. Each repository declares the tracker in one line of its `AGENTS.md`
(`Tracker: Linear — workspace pegasuz · team ENG`). How to write an issue: the
`opening-an-issue` skill in [`pegasuzhq/skills`](https://github.com/pegasuzhq/skills). How the
workspace is configured, and what every label means:
[`pegasuzhq/workspace/linear/`](https://github.com/pegasuzhq/workspace/tree/main/linear).

## Language

English for everything an engineer reads: code, comments, documentation,
commit messages, branch names, issue titles and bodies, pull request titles
and bodies.

Spanish for everything a customer reads: interface copy, site content, SEO.

## Pull requests

- Every change reaches the default branch through a pull request. No direct
  pushes.
- Run the repository's own gates before opening it, and put their output in
  the description. A gate you did not run is reported as not run — never
  assumed green.
- Keep it small. A reviewer who cannot hold the change in their head will
  approve it without reading it.
- The body's first line names the issue: `Closes ENG-123`, or `Part of ENG-123`
  for a partial change. The merge moves the issue to Merged; Done is set by the
  handoff with evidence, never by the merge.
- Rebase merge. Keep the history linear.

## Never

- Commit a secret: no `.env`, no private key, no token, no credential. If you
  find one already committed, report it privately — see `SECURITY.md`.
- Deploy, restart a service or run a migration from a pull request. Those need
  explicit authorisation, every time.
