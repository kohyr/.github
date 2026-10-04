# Kohyr repository defaults

Shared community files and reusable starting configuration for repositories in
the `kohyr` organization. GitHub displays [profile/README.md](profile/README.md)
on the organization profile; this root README explains the repository itself.

## Use and placement

| Path | Purpose |
| --- | --- |
| [CONTRIBUTING.md](CONTRIBUTING.md), [SECURITY.md](SECURITY.md) | Default contribution and private vulnerability-reporting guidance |
| [ISSUE_TEMPLATE](ISSUE_TEMPLATE), [PULL_REQUEST_TEMPLATE.md](PULL_REQUEST_TEMPLATE.md) | Shared issue forms and pull request template |
| [profile/README.md](profile/README.md) | Organization profile content |
| [workflows](workflows) | Workflow examples for CI, CodeQL, releases, and stale issues |
| [dependabot.yml](dependabot.yml), [CODEOWNERS](CODEOWNERS), [FUNDING.yml](FUNDING.yml) | Dependency, ownership, and funding configuration to copy where needed |

Repositories with their own community files use those versions. Copy relevant
configuration into a consuming repository's `.github/` folder and adapt it to
that repository's actual commands. The examples in `workflows/` are source
templates here, not active workflows in this checkout.

Keep shared defaults here and project-specific instructions in the consuming
repo's README. Generated logs, ZIP bundles, and temporary reviews do not belong
in this repository.

## Checks and changes

This repository has no application, package manifest, or build/test command.
Validate edited Markdown, relative links, and copied workflow syntax. Preserve
security reporting, permission requirements, and release controls when adapting
a template; adding a file alone does not prove a remote setting is active.
