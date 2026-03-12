# Contributing

These are private repositories for Australian Food and Fibre's internal data platform. Contributions are limited to authorised team members and partners.

## Getting Started

1. Clone the repository and follow the [Setup Guide](https://github.com/Australian-Food-and-Fibre/data-platform/blob/main/docs/setup-guide.md)
2. Create a feature branch from `main`
3. Make your changes following the conventions below
4. Open a pull request for review

## Conventions

### Language

- Use **Australian English** spelling (organisation, colour, behaviour)

### File Naming

| Type | Convention | Example |
|------|------------|---------|
| Markdown | kebab-case | `azure-setup.md` |
| PowerShell | Verb-Noun PascalCase | `Get-AFFWorkspaces.ps1` |
| Python | snake_case | `detect_ica_deltas.py` |
| SQL | kebab-case or numbered | `00-deploy-full-elt-schema.sql` |

### Code Style

- **Python**: Formatted and linted with [Ruff](https://docs.astral.sh/ruff/) (config in `ruff.toml`)
- **PowerShell**: OTBS preset, `[CmdletBinding()]`, `-WhatIf` support, comment-based help
- **Markdown**: ATX headers, fenced code blocks with language tags
- **SQL**: Uppercase keywords, lowercase identifiers

### Commits

- Use [Conventional Commits](https://www.conventionalcommits.org/) format
- Examples: `feat(gold): add calendar dimension`, `fix(controldb): correct merge key`, `docs: update setup guide`

### Pull Requests

- Keep PRs focused — one logical change per PR
- Include a description of what changed and why
- Ensure linting passes before requesting review

## Fabric Workspace Changes

Changes to Fabric workspace items follow a specific workflow:

1. Make changes in the **Dev** workspace via Fabric portal
2. Commit workspace changes to Git via Fabric Git Integration
3. Open a PR for review
4. After merge, sync to UAT/Prod via deployment pipelines

See [CLAUDE.md](https://github.com/Australian-Food-and-Fibre/data-platform/blob/main/CLAUDE.md#git-integration-workflow) for detailed sync commands.
