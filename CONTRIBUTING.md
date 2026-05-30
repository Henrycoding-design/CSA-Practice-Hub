# Contributing to AP CSA Practice Hub

Thanks for helping improve AP CSA Practice Hub. This project values accuracy, plain explanations, and resources that students can actually use during exam prep.

## Fork Workflow

1. Fork the repository.
2. Create a focused branch from `main`.
3. Make one logical change per pull request.
4. Check formatting and links before submitting.
5. Open a pull request using `.github/PULL_REQUEST_TEMPLATE.md`.

## Branch Naming

Use short kebab-case names with a clear prefix:

- `docs/readme-study-flow`
- `frq/2024-review-update`
- `syntax/recursion-examples`
- `resource/codingbat-links`
- `fix/link-check-issue`

## Contribution Areas

- `docs/*`: repository documentation, release notes, and project guidance.
- `frq/*`: FRQ answer guides, review notes, official links, and templates.
- `syntax/*`: Java syntax explanations, examples, and AP CSA traps.
- `resource/*`: official links, videos, practice sites, IDEs, and textbooks.

The repository uses `frqs/`, `syntax-review/`, and `resources/` as directory names. The category labels above describe the type of contribution.

## Pull Request Requirements

- Link to the related issue when one exists.
- Explain what changed and why it helps students.
- Verify that links work.
- Use fenced code blocks with the correct language, such as `java`.
- Avoid invented sources, fake citations, or AI-hallucinated references.
- Keep official College Board content as links or short summaries; do not copy full prompts.

## Style Guide

- Write for a student who is smart, stressed, and short on time.
- Prefer examples over abstract rules.
- Use AP CSA-compatible Java; avoid features outside the expected course subset.
- Name files in kebab-case, such as `classes-objects.md`.
- Keep headings descriptive and consistent.
- Separate answer logic from mistake analysis when writing FRQ material.

## Review Checklist

- Formatting is readable in Markdown preview.
- Java snippets compile conceptually and use clear variable names.
- New resources are relevant to AP CSA.
- The change matches the existing repository structure.
- No sensitive data, private notes, credentials, or student information is included.
