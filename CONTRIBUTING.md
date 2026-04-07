# Contributing

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change.

## Merge Request Process

1. Create your MR and add reviewers. Owners or contributors of this repository must be added as reviewers.
2. Run pre-commit hooks `pre-commit run -a`.
3. Once all comments and checklist items have been addressed, your contribution will be merged! Merged MRs will be included in the next release. [Semantic release](https://github.com/semantic-release/semantic-release) will be in charge to construct the Release automatically (Tag, CHANGELOG).

## Checklists for contributions

- [ ] Add [semantics prefix](#semantic-pull-requests) to your Commits
- [ ] MR Title and description written in English
- [ ] Run pre-commit hooks `pre-commit run -a`
- [ ] CI is passing (if needed)

## Semantic Pull Requests

To generate changelog, Pull Requests and Commit messages must follow [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) specs below:

- `feat:` for new features
- `fix:` for bug fixes
- `docs:` for documentation and examples
- `refactor:` for code refactoring
- `test:` for tests
- `ci:` for CI purpose
- `chore:` for chores stuff

We use the `chore` prefix to generate a new release and for changelog generation (the label '[skip ci]' allows us to skip CI). It can be used for `chore: update changelog` commit message by example.

We do Squash Merge during the MRs merge. The title of the MR is the commit title (commit type + scope + short description) and the description of the MR is the commit body.
