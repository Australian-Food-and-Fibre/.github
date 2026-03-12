# .github

Organisation-level community health files, issue/PR templates, and default settings for [Australian Food and Fibre](https://github.com/Australian-Food-and-Fibre).

## Contents

| File | Purpose |
|------|---------|
| `profile/README.md` | Organisation profile (visible on org page) |
| `SECURITY.md` | Security vulnerability reporting policy |
| `CONTRIBUTING.md` | Contribution guidelines (inherited by all repos) |
| `CODE_OF_CONDUCT.md` | Code of conduct |
| `.github/ISSUE_TEMPLATE/` | Issue templates (bug, feature, task) |
| `.github/PULL_REQUEST_TEMPLATE.md` | Default PR template |
| `.vscode/` | Default VS Code workspace settings and extensions |
| `.editorconfig` | Cross-editor formatting consistency |
| `.gitignore` | Default ignore patterns |

## How It Works

- **Community health files** (`SECURITY.md`, `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`) are inherited by all repositories in the organisation that don't have their own versions
- **Issue and PR templates** in `.github/` are available when creating issues/PRs in any org repository
- **VS Code settings** and `.editorconfig` serve as reference defaults — copy to individual repos as needed

## Customisation

Individual repositories can override any of these files by creating their own version. Repository-level files always take precedence.
