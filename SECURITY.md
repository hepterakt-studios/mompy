# Security Policy

Mompy is currently in active development.

## Supported versions

Security notes and fixes apply to the latest public release and to the current development version on the `main` branch.

| Version           | Supported |
| ----------------- | --------- |
| Latest release    | ✅         |
| `main` branch     | ✅         |
| Older test builds | ❌         |

## Reporting a vulnerability

Please do not open public issues for serious security problems.

For now, report security concerns directly to the project owner through GitHub contact channels.

When reporting, include:

* what the issue is;
* how it can be reproduced;
* what files or features are affected;
* screenshots or logs, if useful;
* whether the issue exposes user data or local files.

## Local-first security goals

Mompy's first desktop version should:

* avoid online accounts by default;
* avoid passwords unless a real account system exists;
* store profile and progress locally;
* avoid sending user progress to external services;
* avoid committing private files, tokens, installers, or build folders.

## Dependency safety

Before adding a new dependency, check whether it is actually needed.

Prefer simple local code when it is enough for the feature.
