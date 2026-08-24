# Security policy

## Reporting a vulnerability

Report privately through GitHub's **Private vulnerability reporting** on the
affected repository: *Security* → *Report a vulnerability*. It reaches the
Pegasuz security team directly and stays private until a fix ships.

**Do not open a public issue for a security problem.**

Please include reproduction steps, the affected version or commit, and the
impact you believe it has.

## What to expect

- Acknowledgement within one week.
- An assessment and a rough timeline once we have reproduced it.
- Credit in the fix, unless you prefer otherwise.

## Scope

The default branch of each repository is what production runs from and is the
only supported target. Feature branches, forks and archived repositories are
out of scope.

Pegasuz operates multi-tenant systems holding customer business data. Findings
that could expose one tenant's data to another are treated as critical.
