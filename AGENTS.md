# Kohyr .github

Org-level GitHub defaults and the root agent instruction file for Kohyr
repositories. This file is read natively by Codex, Cursor, Kilo Code, Grok and
GitHub Copilot; `CLAUDE.md` imports it for Claude Code, so there is one source
of truth. Per-repo `AGENTS.md` files add repo-specific rules and never relax
these.

## Shared policy

Kohyr follows the same kit as the alawein account so both behave identically.
The canonical rules live in [alawein/.github](https://github.com/alawein/.github):

- [Agent rules](https://github.com/alawein/.github/blob/main/docs/system/agents.md)
- [Delivery rules](https://github.com/alawein/.github/blob/main/docs/system/delivery.md)
- [Reviewer policy](https://github.com/alawein/.github/blob/main/docs/system/reviewers.md)
- [Per-repo AGENTS template](https://github.com/alawein/.github/blob/main/templates/agent/AGENTS.template.md)

Do not copy those rules into this file. Cite their stable rule IDs.

## Start here

1. Read the repo's own `AGENTS.md`, then this file.
2. Run `git status` and the repo's check command before any change.
3. Report any check that could not run as "not run" with the reason.

## Remote work

- Claude Code, ChatGPT/Codex, Cursor, Grok and Kilo Code Cloud Agents may work
  remotely. Each task names the repository, target branch and scope.
- Gated actions need named owner approval each time: send, spend, publish,
  purge or delete, commit, push, merge, open a PR, rotate a secret, or change
  any remote setting. Checks and review approval never supply merge permission.
- One writer per branch. Parallel agents use separate branches.
- Never open, print or copy secrets, credentials or `.env` files.

## Review

Follow the reviewer policy linked above. Findings need actionable evidence and
never authorize a gated action. Mark unobserved account or enforcement state
UNVERIFIED.

## Verify before done

Run the repo's check command, record the command and exit result, and never
claim an unrun check passed. Stage named paths only, never `git add -A`.
