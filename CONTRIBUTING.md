# Contributing to Kohyr

Thank you for your interest in contributing!

## Getting started

1. Fork and clone the repo
2. Create a feature branch: `git checkout -b feat/your-feature`
3. Make your changes and add tests
4. Run `make check` (or `pnpm test` / `python -m pytest`) to verify
5. Commit following [Conventional Commits](https://www.conventionalcommits.org/)
6. Push and open a pull request

## Commit format

```
type(scope): short description

# Types: feat, fix, docs, refactor, perf, test, build, ci, chore
# Breaking change: feat!: or add BREAKING CHANGE: in footer
```

## Code style

- **Python**: formatted with `ruff`, type-checked with `mypy`
- **TypeScript/JS**: formatted with Prettier, linted with ESLint
- Write tests for any new functionality
- Keep PRs focused on a single concern

## Questions?

Use [GitHub Discussions](https://github.com/orgs/kohyr/discussions) for questions, not Issues.

## License

By contributing, you agree your contributions will be licensed under the [MIT License](LICENSE).
