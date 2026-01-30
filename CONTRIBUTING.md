# Contributing to AdTecher

Thank you for your interest in contributing to AdTecher projects! This document provides guidelines and information for contributors.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Development Workflow](#development-workflow)
- [Coding Standards](#coding-standards)
- [Submitting Changes](#submitting-changes)
- [Review Process](#review-process)

## Code of Conduct

All contributors are expected to adhere to our [Code of Conduct](CODE_OF_CONDUCT.md). Please read it before contributing.

## Getting Started

1. **Fork the repository** you want to contribute to
2. **Clone your fork** locally
3. **Set up your development environment** following the project's README
4. **Create a new branch** for your changes

```bash
git checkout -b feature/your-feature-name
# or
git checkout -b fix/your-bug-fix
```

## Development Workflow

### Branch Naming Convention

- `feature/` - New features
- `fix/` - Bug fixes
- `docs/` - Documentation changes
- `refactor/` - Code refactoring
- `test/` - Test additions or modifications

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
```

## Coding Standards

We maintain detailed coding standards in our documentation:

- **[Python Standards](https://github.com/AdTecher/vulcan-enterprise-api/blob/main/docs/development/CODING_STANDARDS.md)** - For Python projects
- **[Project Structure](https://github.com/AdTecher/vulcan-enterprise-api/blob/main/docs/development/PROJECT_STRUCTURE.md)** - For folder organization
- **[Testing Guidelines](https://github.com/AdTecher/vulcan-enterprise-api/blob/main/docs/development/TESTING.md)** - For writing tests

### Key Principles

1. **Type hints** are required for all Python code
2. **Tests** are required for new features
3. **Documentation** should be updated with code changes
4. **Code formatting** is enforced via pre-commit hooks

### Running Quality Checks

```bash
# Format code
make format

# Run linter
make lint

# Run type checking
make type-check

# Run all checks
make check
```

## Submitting Changes

1. **Ensure all tests pass** locally
2. **Update documentation** if needed
3. **Push your branch** to your fork
4. **Open a Pull Request** against the `main` branch

### Pull Request Guidelines

- Use the PR template provided
- Link related issues using keywords (`Fixes #123`, `Closes #456`)
- Request review from appropriate team members
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

## Questions?

If you have questions about contributing, please:

1. Check existing documentation
2. Search open/closed issues
3. Open a new issue with your question

Thank you for contributing to AdTecher!
