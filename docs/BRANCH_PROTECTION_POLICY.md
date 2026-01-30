# Branch Protection Policy

## Overview

This document describes branch protection rules enforced across all AdTecher repositories. The level of enforcement depends on repository visibility and the organization's GitHub plan.

## Rules for `main` Branch

All repositories follow these rules for the `main` branch:

| Rule | Description |
|------|-------------|
| No direct pushes | All changes must go through a pull request |
| Minimum 1 approval | At least one reviewer must approve before merge |
| Dismiss stale approvals | Approvals are dismissed when new commits are pushed |
| Conventional commit titles | PR titles must follow `type(scope): description` format |
| Branch naming convention | Branches must use `feature/`, `fix/`, `chore/`, or `docs/` prefix |
| PR description required | Minimum 50 characters of non-template content |
| Squash and merge | Preferred merge strategy for clean history |

## Enforcement Status

### Public repositories (.github)

Branch protection is **enforced via GitHub branch protection rules**:

- Require pull request reviews before merging (1 approval)
- Dismiss stale pull request approvals on new pushes
- Restrict pushes to `@AdTecher/leadership`

### Private repositories (Free plan)

Branch protection rules are **not available** on the GitHub Free plan for private repositories. Instead, compliance is enforced via a **CI workflow** (`pr-standards.yml`) that:

- Validates PR description length
- Checks for linked issues
- Validates branch naming convention
- Validates conventional commit format in PR title
- Posts a compliance summary comment on each PR
- Fails the status check if standards are not met

While this does not prevent direct pushes to `main`, the failed status check is visible to all contributors as a clear signal.

## Upgrade Path

When the organization upgrades to the GitHub Team plan ($4/user/month), the following will be enabled on private repositories:

- [ ] Branch protection rules (matching public repo settings)
- [ ] Required status checks (pr-standards workflow must pass)
- [ ] CODEOWNERS enforcement
- [ ] Restrict push access to specific teams

## Related

- [Contributing Guide](https://github.com/AdTecher/.github/blob/main/CONTRIBUTING.md)
- [PR Template](https://github.com/AdTecher/.github/blob/main/PULL_REQUEST_TEMPLATE.md)
