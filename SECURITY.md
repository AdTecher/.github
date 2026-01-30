# Security Policy

## Supported Versions

| Project | Supported Versions |
| ------- | ------------------ |
| Project Vulcan | Latest release |
| Vulcan Enterprise API | Latest release |
| KeyTakeAways Dashboard | Latest release |

## Reporting a Vulnerability

We take security vulnerabilities seriously. If you discover a security issue, please report it responsibly.

### How to Report

**DO NOT** open a public GitHub issue for security vulnerabilities.

Instead, please report security vulnerabilities by emailing:

**security@adtecher.com**

Include the following information:

1. **Description** of the vulnerability
2. **Steps to reproduce** the issue
3. **Potential impact** of the vulnerability
4. **Suggested fix** (if you have one)

### What to Expect

- **Acknowledgment**: We will acknowledge receipt within 48 hours
- **Assessment**: We will assess the vulnerability and determine its severity
- **Updates**: We will keep you informed of our progress
- **Resolution**: We aim to resolve critical vulnerabilities within 7 days
- **Credit**: We will credit you in the security advisory (unless you prefer anonymity)

### Scope

This security policy applies to:

- All repositories under the AdTecher organization
- Our production services and APIs
- Infrastructure and deployment configurations

### Out of Scope

- Vulnerabilities in third-party dependencies (please report to the respective maintainers)
- Social engineering attacks
- Physical security issues

## Security Best Practices

For contributors, please follow these security guidelines:

1. **Never commit secrets** - Use environment variables and secret management
2. **Keep dependencies updated** - Regularly update to patched versions
3. **Follow least privilege** - Request only necessary permissions
4. **Validate inputs** - Always sanitize and validate user inputs
5. **Use HTTPS** - Ensure all communications are encrypted

## Security Features

Our projects implement:

- Row-Level Security (RLS) for multi-tenant data isolation
- AWS Secrets Manager for credential management
- Regular security audits and penetration testing
- Automated dependency vulnerability scanning

Thank you for helping keep AdTecher and our users safe!
