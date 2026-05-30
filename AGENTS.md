# AI Agent & Developer Guidelines

This document outlines the standards and workflows for maintaining the **CSA-Practice-Hub**. Following these guidelines ensures that all contributions remain consistent, high-quality, and pass automated CI checks.

## 🛠 Maintenance Workflows

### 1. Markdown Linting
We use `markdownlint` to maintain formatting consistency.
- **Command**: `npx markdownlint-cli2 "**/*.md" "#node_modules"`
- **Auto-fix**: `npx markdownlint-cli2 "**/*.md" "#node_modules" --fix`
- **Standard**: All tables must be aligned. Headings and lists must have appropriate blank lines.

### 2. Spell Checking
We use `cspell` with a custom configuration to handle technical AP CSA terminology.
- **Command**: `npx cspell "**/*.md" --no-progress`
- **Configuration**: `.cspell.json`
- **Adding Words**: If a technical term is flagged as an error but is correct, add it to the `words` array in `.cspell.json`.
- **Ignoring Code**: Inline code (`` ` ` ``) and blocks (`` ``` ``` ``) are automatically ignored by regex patterns in `.cspell.json`.

## 🤖 Instructions for AI Agents

When editing files in this repository:
1. **Always Validate**: After any modification, run the lint and spell check commands listed above.
2. **Respect Templates**: Maintain the structure of files in the `/templates` directory.
3. **No Hidden Logic**: Avoid using HTML tags for formatting unless absolutely necessary; stick to standard Markdown.
4. **Table Alignment**: Ensure all Markdown tables are manually aligned if the auto-fixer fails to do so.

## 🚀 Pre-Commit Checklist

Before pushing changes or opening a PR, ensure:
1. [ ] `npx markdownlint-cli2` returns 0 errors.
2. [ ] `npx cspell` returns 0 errors.
3. [ ] All Java code snippets in Markdown are syntactically correct according to the AP CSA subset.
