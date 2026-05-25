# Contributing to AP CSA Practice Hub

Thank you for your interest in contributing! Our goal is to provide high-quality, practical resources for AP CSA students. We value clarity, accuracy, and adherence to the AP Java Subset.

## How to Contribute

1.  **Find an Issue**: Check our [Issue Tracker](https://github.com/your-repo/issues) for open tasks or "Good First Issues."
2.  **Submit a New FRQ**: Use the template in `/frqs/template/` to ensure consistency.
3.  **Report a Bug/Trap**: Found a common student mistake? Add it to `/syntax-review/common-traps.md` or the `/error-log/`.
4.  **Formatting**: Ensure all Java code strictly follows the **AP Java Subset** (e.g., using `ArrayList` methods correctly, no `var` keyword, etc.).

## File Naming Conventions

-   Directories: `kebab-case` (e.g., `syntax-review`)
-   Markdown Files: `kebab-case.md` (e.g., `common-traps.md`)
-   FRQs: `YYYY-qN-title.md` (e.g., `2024-q1-word-games.md`)

## Code Snippet Standards

All code blocks must specify the language as `java` and follow clean formatting:

```java
// Good example: Clear and commented
public class Example {
    public static void main(String[] args) {
        System.out.println("Hello, AP CSA!");
    }
}
```

## Templates

### Adding a Syntax Trap
When adding a new trap to `common-traps.md`, use this structure:
- **The Trap**: Short description of the mistake.
- **The "Why"**: Explanation of the underlying logic error.
- **The Fix**: Correct code snippet.

### Adding an FRQ Walkthrough
Please use the gold-standard template located at `/frqs/template/frq-walkthrough-template.md`.

---
Questions? Feel free to open a discussion or reach out to the maintainers.
