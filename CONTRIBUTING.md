# Contributing

The baseline for every Pegasuz repository. A repository that ships its own
`CONTRIBUTING.md` overrides this one — read that instead.

## Before you start

Read the repository's `AGENTS.md` and `README.md`. Anything specific — how to
run it, which gates must pass, what not to touch — lives there, not here.

## Branches and commits

- Branch from the default branch: `feat/<topic>`, `fix/<topic>`,
  `docs/<topic>`, `chore/<topic>`.
- [Conventional commits](https://www.conventionalcommits.org): `feat:`, `fix:`,
  `docs:`, `chore:`, `refactor:`, `test:`.
- One reason per commit. If the message needs an "and", it is two commits.
- Push your work. Servers deploy from the remote; unpushed work does not exist.

## Language

English for everything an engineer reads: code, comments, documentation,
commit messages, branch names, pull request titles and bodies.

Spanish for everything a customer reads: interface copy, site content, SEO.

## Pull requests

- Every change reaches the default branch through a pull request. No direct
  pushes.
- Run the repository's own gates before opening it, and put their output in
  the description. A gate you did not run is reported as not run — never
  assumed green.
- Keep it small. A reviewer who cannot hold the change in their head will
  approve it without reading it.
- Rebase merge. Keep the history linear.

## Never

- Commit a secret: no `.env`, no private key, no token, no credential. If you
  find one already committed, report it privately — see `SECURITY.md`.
- Deploy, restart a service or run a migration from a pull request. Those need
  explicit authorisation, every time.
