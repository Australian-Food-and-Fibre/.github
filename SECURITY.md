# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability in any Australian Food and Fibre repository, please report it responsibly.

**Do not** open a public issue for security vulnerabilities.

### How to Report

1. Email **bwalsh@australianfoodandfibre.com.au** with details of the vulnerability
2. Include steps to reproduce, affected components, and potential impact
3. Allow reasonable time for a response before any public disclosure

### What to Expect

- Acknowledgement within 3 business days
- Assessment and remediation plan within 10 business days
- Notification when the issue is resolved

## Supported Versions

Only the latest version of each repository's `main` branch is actively maintained.

## Security Practices

- All secrets and credentials are stored in Azure Key Vault — never in code
- Service principal authentication uses certificate or client secret via `.env.local` (gitignored)
- Fabric workspace access is controlled via Entra ID security groups
- CodeQL security scanning is enabled on repositories
- Dependabot alerts are monitored for dependency vulnerabilities
