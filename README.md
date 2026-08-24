# .github

Organisation-wide defaults for every repository under `pegasuzhq`.

GitHub applies the files here to any repository that does not provide its own.
A repository that ships its own `CONTRIBUTING.md`, `SECURITY.md` or issue
templates overrides these — the nearest file always wins.

| File | Applies to |
|---|---|
| `SECURITY.md` | every repo without one |
| `CONTRIBUTING.md` | every repo without one |
| `SUPPORT.md` | every repo without one |
| `.github/PULL_REQUEST_TEMPLATE.md` | every repo without one |
| `.github/ISSUE_TEMPLATE/` | every repo with an empty `ISSUE_TEMPLATE` folder |
| `profile/README.md` | the public organisation page |

## What is deliberately not here

- **`CODEOWNERS`** — not an inheritable file. Every repository needs its own.
- **Workflows** — not inheritable either. They live in the repo that runs them.
- **`LICENSE`** — GitHub does not support default licences.
- **Anything internal** — this repository is public, which GitHub requires for
  the defaults to apply. Tenant names, deploy paths and infrastructure detail
  belong in `pegasuzhq/workspace` and `pegasuzhq/infra`, both private.
