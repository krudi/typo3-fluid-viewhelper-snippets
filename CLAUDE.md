# TYPO3 Fluid ViewHelper Snippets

VS Code extension — TYPO3 Fluid ViewHelper snippets and TypoScript/TSConfig syntax highlighting for `.fluid.html` files.

@AGENTS.md

## For Claude Code

### Rules loaded automatically

| Rule file | Applied to |
|-----------|---|
| `.ai/rules/vscode-extension.md` | `**/*.json`, `package.json` |

### Constraints

- No build step — snippet JSON files are consumed directly by VS Code
- Test changes manually with `F5` (Extension Development Host) — no automated tests
- Commits use conventional commits format (see global `AGENTS.md`)
- All snippet namespaces: `f:*`, `be:*`, `core:*`, `formvh:*`, `cb:*` — keep consistent
- `package.json` `engines.vscode` defines minimum VS Code compatibility — do not lower it without testing
