# Bar Inventory KMP

Mobile client for **Bar Inventory**, an agentic software development project.

This repository will hold the Kotlin Multiplatform app targeting Android and
iOS. No application code has been generated yet. It will be added through the
project's agentic workflow.

## Technology stack

- Language: Kotlin
- Platform: Kotlin Multiplatform (shared code for Android and iOS)
- Targets: Android, iOS
- Backend: [bar-inventory-api](https://github.com/kaanf/bar-inventory-api) (Kotlin + Spring Boot)

## Branch strategy

- `main`: production / release branch
- `dev`: integration branch
- `feat/*`: feature branches, created from `dev` and merged back into `dev` via pull request

Releases are promoted from `dev` to `main`.

## Related repositories

| Repository | Purpose |
| --- | --- |
| [bar-inventory](https://github.com/kaanf/bar-inventory) | Central workspace: product design, PRD, architecture and shared CI/workflow |
| [bar-inventory-api](https://github.com/kaanf/bar-inventory-api) | Kotlin + Spring Boot backend |
| [bar-inventory-kmp](https://github.com/kaanf/bar-inventory-kmp) | Kotlin Multiplatform mobile app (this repository) |

Each repository is independent with its own Git history. Product and
architecture decisions live in the central workspace repository. This
repository implements the mobile side of those decisions.

## Secrets

Never commit credentials, tokens, signing keys (keystores, `.p12`,
provisioning profiles) or environment files. Keep them in local, git-ignored
files or in CI secret storage.
