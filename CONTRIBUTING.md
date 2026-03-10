# Contributing to Next.js App Router Snippets

Thank you for your interest in contributing to this project! Your help is greatly appreciated.

## How to Contribute

1. **Fork the repository** and create your branch from `main`.
2. **Make your changes** (add new snippets, fix bugs, improve documentation, etc.).
3. **Use Conventional Commits** when writing commit messages (details below).
4. **Test your changes** to ensure they work as expected.
5. **Submit a pull request** with a clear description of your changes.

## Guidelines

- Follow the existing code style and structure.
- For new snippets, provide:
  - a clear **prefix**
  - a meaningful **description**
  - a complete and correct **body**
- Update documentation if necessary.
- Reference related issues or discussions in your pull request.

### Commit Message Guidelines (Conventional Commits)

This project follows the **Conventional Commits** standard to keep the commit history clean and meaningful.

#### Format

```
<type>(optional scope): <short description>
```

#### Allowed types

| Type | When to use it |
| ---- | -------------- |
| feat | Adding a new snippet |
| fix | Fixing a snippet |
| docs | Updating documentation |
| refactor | Code refactoring without changing behavior |
| style | Formatting changes (no logic changes) |
| chore | Maintenance tasks, tooling updates |
| test | Adding or updating tests |

#### Examples

```
feat(snippets): add snippet for dynamic route generation
fix(snippets): correct import path in middleware snippet
chore(ci/fix): repair failing build step
docs: update README with installation instructions
refactor: simplify snippet generation logic
```

##### Breaking change

```json
...
"body": [
  "import { NextResponse } from 'next/server'",
  "",
  "export async function GET() {",
  "  return NextResponse.json({ message: 'Hello' })",
  "}"
]
...
```

* The new snippet requires an import that previously wasn’t needed.
* The behavior of the snippet changes, not just formatting.

```
feat(snippets)!: update route handler snippet to use NextResponse.json
```

### Snippet Style Guide

This project uses a pattern‑oriented approach for all snippets.
Each snippet must clearly indicate where it can be used, what pattern it represents, and how it fits into the App Router architecture.

Please make sure your contribution aligns with the rules below.

#### Prefix

Must be short, descriptive, and consistent with existing prefixes.

Common patterns include:
* `next-` for general Next.js snippets
* `app-` for App Router–related snippets
* `route-` for route handlers
* `api-` for API route handlers
* `layout-` for layouts
* `meta-` metadata patterns

Prefixes must be unique and must not conflict with existing ones.

> [!TIP]
> Avoid overly generic names.

#### Description

* Should be a short, action‑oriented sentence.
* Use imperative form (e.g., “Create…”, “Generate…”, “Define…”).
* Keep it concise and meaningful.

#### Include

Every snippet must include an `include` field describing:
* Where the snippet can be used (eg. app directory, lib catalog)
* What pattern it represents (e.g., dynamic route, loading, metadata)

### Body Formatting Rules

* Use TypeScript and React syntax.
* Follow the formatting style of existing snippets.
* Each line must be a separate string in the body array.
* Use placeholders:
    * $1, $2 for cursor positions
    * ${TM_FILENAME_BASE} when referencing the file name
* Avoid any imports.
* Follow App Router conventions (server components by default, etc.).
* Use `\t` for indentations

### Avoiding Duplicates

Before adding a snippet:
* Check if a similar pattern already exists.
* If your snippet extends an existing pattern, consider updating the original instead.

### Testing Your Snippet

1. Reload VS Code (`Developer: Reload Window`).
2. Trigger the snippet using its prefix.
3. Verify:
    * It appears in IntelliSense.
    * The generated code is valid.
    * Placeholders work correctly.
    * It works in .tsx files.
    * The include field accurately describes its usage.
    * It does not conflict with existing prefixes.

### File Placement

All TypeScript React snippets must be added to: `snippets/typescriptreact/nextjs.code-snippets`

## Reporting Issues

If you find a bug or have a feature request, please [open an issue](https://github.com/hedge-code/nextjs-app-router-snippets/issues) with as much detail as possible.

## 🛠️ Continuous Integration & Release Process

This project uses GitHub Actions to automate building, testing, and releasing the extension.
### Build Workflow
* Runs automatically on every push to dev and main.
* Builds the VS Code extension and ensures it compiles correctly.
* Uploads a .vsix artifact that can be downloaded for testing.

### Release Workflow
* Runs automatically when a new version tag (v*) is pushed.
* Generates a changelog for the release.
* Publishes the extension to the VS Code Marketplace.
* Creates a GitHub Release with the packaged .vsix.

### Changelog Workflow
* Runs on version tags (v*).
* Updates the CHANGELOG.md file in the main branch.
* Contributors do not need to trigger these workflows manually.  
* Just open a pull request — maintainers handle tagging and releasing.

## Code of Conduct

Please be respectful and considerate in all interactions. See [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for details.

---

Thank you for helping make this project better!
