---
description: VS Code extension conventions — snippets, grammar, package.json manifest
globs: ["**/*.json", "**/*.yaml", "**/*.tmLanguage.json"]
alwaysApply: false
---

# VS Code Extension Conventions

## Snippets

- Each snippet needs a unique `prefix` — check for conflicts before adding
- Use tab stops in order: `$1`, `$2`, ... `$0` for final cursor position
- Use `${1:placeholder}` for meaningful placeholder text
- Test every snippet with `F5` (Extension Development Host) before committing

## Package manifest (`package.json`)

- `engines.vscode` must match the minimum VS Code version you support — don't bump unnecessarily
- New snippet files must be registered under `contributes.snippets`
- New grammar files must be registered under `contributes.grammars`

## No build step

Changes to snippets and grammar files are immediately testable — no compile step needed.
Press `F5` in VS Code to open an Extension Development Host and test live.

## Commit format

Use root conventional commits format — this project has no `CONTRIBUTING.md` override.
