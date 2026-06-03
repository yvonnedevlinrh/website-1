# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| latest  | :white_check_mark: |

## Reporting a Vulnerability

If you discover a security vulnerability in this project, please report it
responsibly. **Do not open a public GitHub issue.**

Instead, please use one of the following methods:

1. **GitHub Security Advisory** (preferred): Use the
   [private vulnerability reporting](https://github.com/complytime/website/security/advisories/new)
   feature on this repository.

2. **Email**: Send details to the maintainers listed in the repository's
   `MAINTAINERS` file or reach out via the organization contact.

### What to include

- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Suggested fix (if any)

### Response timeline

- **Acknowledgment**: Within 5 business days of report
- **Assessment**: Within 10 business days
- **Fix or mitigation**: Depending on severity, typically within 30 days

## Security Best Practices

This project follows supply-chain security best practices:

- GitHub Actions are pinned to full SHA digests
- Dependencies are monitored via Dependabot and OSV-Scanner
- OpenSSF Scorecard checks run on every push and on a daily schedule
