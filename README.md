# Next.js App Router Snippets

Snippets for faster and consistent development with the Next.js App Router.

## Features

- **15+ Snippets** – Coverage for all major App Router file types
- **Context-Aware** – Snippets appear only in matching file patterns
- **App Router‑Optimized** — Pages, layouts, error boundaries, metadata, loading states
- **TypeScript‑Native** – Designed for `.tsx` files
- **Best‑Practice Templates** – Encourages idiomatic Next.js structure
- **Time Saving** – Reduce boilerplate and follow Next.js best practices

## Usage

1. Install the extension from the VS Code Marketplace or manually from the VSIX package.
2. Open a TypeScript React (`.tsx`) file in your Next.js project.
3. Type a snippet prefix (e.g., `appRoutePage`, `appRouteNotFound`).
4. Select the snippet from IntelliSense.
5. The snippet will expand into a ready-to-use code template.

### Context-Aware Snippets

> **Note:** Not every snippet is available in every `.tsx` file. Each snippet is context-aware and will only appear in files that match specific patterns. For example, a snippet for a `not-found.tsx` page will only be suggested in files named `not-found.tsx` within the `app` directory. This keeps IntelliSense clean and ensures snippets appear only where they make sense.

#### Example Snippet Prefixes & Where They Work

| Prefix | Where it works |
| ------ | -------------- |
| `appRouteNotFound` | `**/app/**/not-found.tsx` |
| `appRouteUnauthorized` | `**/app/**/unauthorized.tsx` |
| `appRouteForbidden` | `**/app/**/forbidden.tsx` |
| `appRouteError` | `**/app/**/error.tsx` |
| `appRouteLoading` | `**/app/**/loading.tsx` |
| `appRoutePage` | `**/app/**/page.tsx` or `**/app/**/[slug]/page.tsx` |
| `appRouteSearchPage` | `**/app/**/page.tsx` or `**/app/**/[slug]/page.tsx` |
| `appRouteLayout` | `**/app/**/layout.tsx` |
| `appRouteMetadata` | `**/app/**/page.tsx` or `**/app/**/layout.tsx` |
| `appRouteStaticParams` | `[slug]/page.tsx`, `[slug]/layout.tsx`, or `[slug]/route.ts` |
| `appRouteAction` | `**/app/**/page.tsx` , `**/lib/**/*.ts`, `**/app/**/actions.ts` or `**/actions/**/*.ts` |
| `appRouteClientComponent` | `**/ui/**/*.tsx`, `**/*provider.tsx` or `**/components/**/*.tsx` |

See the full list of filters and prefixes in the [snippets file](snippets/typescriptreact/nextjs.code-snippets).

## Requirements

- Visual Studio Code v1.109.0 or higher
- Next.js project using the App Router

## Installation

### From VS Code Marketplace

1. Open VS Code
2. Go to the Extensions view (`Ctrl+Shift+X` / `Cmd+Shift+X`)
3. Search for `Next.js App Router Snippets`
4. Click Install

### Manual Installation from VSIX

1. Download the latest `.vsix` file from [Releases](https://github.com/hedge-code/nextjs-app-router-snippets/releases)
2. In VS Code, press `Ctrl+Shift+P` and run `Extensions: Install from VSIX...`
3. Select the downloaded file and click Open

## Contributing

Contributions are welcome. Please read the [Contributing Guide](CONTRIBUTING.md) for details on:

- reporting bugs
- requesting new snippets or improvements
- submitting pull requests
- following code standards and project structure

## Support

- 🐛 [Issues](https://github.com/hedge-code/nextjs-app-router-snippets/issues)
- 💡 [Feature Requests](https://github.com/hedge-code/nextjs-app-router-snippets/issues)
- 📄 [Changelog](CHANGELOG.md)

## License

This project is licensed under the [MIT License](LICENSE) – see the [LICENSE](LICENSE) file for details.


_Maintained by the community. Contributions are welcome._
