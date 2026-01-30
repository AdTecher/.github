# Contributing to AdTecher

Thank you for your interest in contributing to AdTecher projects! This document provides guidelines and information for contributors across all repositories in the organization.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Active Repositories](#active-repositories)
- [Getting Started](#getting-started)
- [Development Workflow](#development-workflow)
- [Coding Standards](#coding-standards)
- [Labels](#labels)
- [Submitting Changes](#submitting-changes)
- [Review Process](#review-process)
- [Team Structure](#team-structure)

## Code of Conduct

All contributors are expected to adhere to our [Code of Conduct](CODE_OF_CONDUCT.md). Please read it before contributing.

## Active Repositories

| Repository | Description |
| ---------- | ----------- |
| vulcan-enterprise-api | Backend API service |
| adtecher-website | Public-facing website |
| KeyTakeAways-dashboard | Analytics dashboard |
| vulcan-demo | Demo / showcase application |

> Archived repos (Project-Vulcan, Project-Canary, Project-Canary-mvp, adtecher-custom-ad-generator) are read-only and not accepting contributions.

## Getting Started

1. **Fork the repository** you want to contribute to
2. **Clone your fork** locally
3. **Set up your development environment** following the project's README
4. **Create a new branch** for your changes (see naming convention below)

## Development Workflow

### Branch Naming Convention

All repositories in the org follow a standardized branch naming convention:

- `feature/` — New features
- `fix/` — Bug fixes
- `chore/` — Maintenance, dependency updates, CI changes
- `docs/` — Documentation changes

```bash
git checkout -b feature/your-feature-name
git checkout -b fix/your-bug-fix
git checkout -b chore/update-dependencies
git checkout -b docs/improve-readme
```

### Commit Messages

Follow conventional commits format:

```
type(scope): description

[optional body]

[optional footer]
```

**Types**: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

**Examples**:
```
feat(api): add tenant lifecycle management endpoint
fix(dashboard): resolve chart rendering issue on mobile
docs(readme): update installation instructions
chore(deps): bump fastapi to 0.110
```

## Coding Standards

### Key Principles

1. **Type hints / type safety** are expected in all code (Python type hints, TypeScript strict mode, etc.)
2. **Tests** are required for new features
3. **Documentation** should be updated alongside code changes
4. **Code formatting** is enforced via pre-commit hooks or CI checks

### Running Quality Checks

Each repository may have its own tooling. Common patterns:

```bash
# Format code
make format

# Run linter
make lint

# Run type checking
make type-check

# Run tests
make test

# Run all checks
make check
```

Refer to the individual repository's README or Makefile for exact commands.

## Labels

All repositories use a standardized label set for issues and pull requests:

| Category | Labels |
| -------- | ------ |
| Type | `bug`, `feature`, `enhancement`, `chore`, `docs` |
| Priority | `priority: critical`, `priority: high`, `priority: medium`, `priority: low` |
| Status | `status: in-progress`, `status: review-needed`, `status: blocked` |
| Area | `area: frontend`, `area: backend`, `area: infra`, `area: docs` |

When opening issues or PRs, please apply the appropriate labels.

## Submitting Changes

1. **Ensure all tests pass** locally
2. **Update documentation** if needed
3. **Push your branch** to your fork
4. **Open a Pull Request** against the `main` branch of the upstream repo

### Pull Request Guidelines

- Use the PR template provided (if available)
- Link related issues using keywords (`Fixes #123`, `Closes #456`)
- Request review from the appropriate team (see below)
- Respond to review feedback promptly

## Review Process

1. **Automated checks** run on every PR (CI/CD, linting, tests)
2. **Code review** by at least one team member
3. **Approval** required before merging
4. **Squash and merge** is the preferred merge strategy

### Review Checklist

Reviewers will check for:

- [ ] Code follows our coding standards
- [ ] Tests are included and passing
- [ ] Documentation is updated
- [ ] No security vulnerabilities introduced
- [ ] Performance implications considered

## Team Structure

Contributions are reviewed by the relevant team:

| Team | Area |
| ---- | ---- |
| **Engineering** | Cross-cutting concerns, architecture |
| **Backend** | API services, data layer, infrastructure |
| **Frontend** | Website, dashboard, UI/UX |
| **Leadership** | Strategy, releases, org-wide decisions |

When in doubt, request a review from the **Engineering** team.

## Questions?

If you have questions about contributing, please:

1. Check existing documentation in the relevant repository
2. Search open and closed issues
3. Open a new issue with your question

Thank you for contributing to AdTecher!