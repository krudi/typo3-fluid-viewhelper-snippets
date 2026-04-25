# TYPO3 Fluid ViewHelper Snippets

VS Code extension providing TYPO3 Fluid ViewHelper snippets and TypoScript/TSConfig syntax highlighting for `.fluid.html` files.

## Stack

- VS Code extension (JSON/YAML snippets, tmGrammer)
- No package manager / build step

## Key paths

- `snippets/` — snippet definition files (JSON)
- `syntaxes/` — TextMate grammar files for syntax highlighting
- `package.json` — extension manifest (contributes, activation events)

## Covered namespaces

- `f:*` — Fluid core ViewHelpers
- `be:*` — Backend ViewHelpers
- `core:*` — Core ViewHelpers
- `formvh:*` — Form ViewHelpers
- `cb:*` — Custom/third-party ViewHelpers

## Onboarding

**Prerequisites:** VS Code, Node.js (for packaging only).

1. Open the project folder in VS Code
2. Press `F5` to launch an Extension Development Host with the extension loaded
3. Open a `.html` file and type `f:` to verify Fluid snippets appear

No dependencies to install — this extension has no build step.

---

## Testing

- Test manually in VS Code with `F5` after every snippet or syntax change
- Verify tab stops work correctly (`Tab` cycles through `$1`, `$2`, etc.)
- Check `package.json` `engines.vscode` compatibility when updating VS Code API usage
- Before publishing: run `vsce package` and install the `.vsix` to test the packaged extension

---

## Publishing

1. Bump version in `package.json`
2. `vsce package` — creates a `.vsix` file
3. Install locally to verify: `code --install-extension typo3-fluid-viewhelper-snippets-x.y.z.vsix`
4. `vsce publish` — publish to VS Code Marketplace

---

## Notes

- Snippets use tab stops (`$1`, `$2`, ...) — test in VS Code after changes
- `package.json` `engines.vscode` must stay compatible with the minimum VS Code version
- No build step — changes to snippets/syntax are immediately testable with `F5` in VS Code

---

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
