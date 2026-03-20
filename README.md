# Dependabot Example

A minimal example repo showing how to configure [Dependabot](https://docs.github.com/en/code-security/dependabot) for a multi-project monorepo.

## How it works

- Dependabot runs weekly and checks each service for outdated dependencies
- Updates are grouped into a single PR per ecosystem/directory
- PRs are automatically labelled by ecosystem (e.g. `javascript`, `dotnet`, `java`, `ci`)
- Open PR limit is capped at 3 per ecosystem

See [`.github/dependabot.yml`](.github/dependabot.yml) for the full configuration.
