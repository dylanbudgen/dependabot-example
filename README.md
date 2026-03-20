# Dependabot Example

A minimal example repo showing how to configure [Dependabot](https://docs.github.com/en/code-security/dependabot) for a multi-project monorepo.

## What's included

| Service | Ecosystem | Path |
|---------|-----------|------|
| Website | npm | `services/website` |
| Backend (dotnet) | nuget | `services/backend-dotnet` |
| Backend (java) | maven | `services/backend-java` |
| CI | github-actions | `/` |

## How it works

Dependabot runs weekly and opens grouped PRs for each service — one PR per ecosystem/directory with all dependency updates bundled together. A CI workflow validates each project on every PR.

See [`.github/dependabot.yml`](.github/dependabot.yml) for the full configuration.
