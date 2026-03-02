
# Next.js App Router Snippets

Supercharge your Next.js workflow with snippets crafted for the App Router era.

## Features

- **15+ Snippets** – Comprehensive coverage for all major Next.js App Router file types
- **Context-Aware** – Snippets only appear in relevant files, keeping your suggestions clean and focused
- **Production Ready** – Scaffolds for pages, layouts, error boundaries, metadata, loading states, and more
- **TypeScript First** – Native support for TypeScript/React (`.tsx`) files
- **Time Saving** – Reduce boilerplate and follow Next.js best practices out of the box


## Usage

1. Install this extension from the VS Code Marketplace or manually from the VSIX package.
2. Open a TypeScript React (`.tsx`) file in your Next.js project.
3. Type a snippet prefix (e.g., `appRoutePage`, `appRouteNotFound`) and select the desired snippet from the suggestions.
4. The snippet will expand into a ready-to-use code template.

### Context-Aware Snippets

> **Note:** Not every snippet is available in every `.tsx` file. Each snippet is context-aware and will only appear in files that match specific patterns. For example, a snippet for a `not-found.tsx` page will only be suggested in files named `not-found.tsx` within the `app` directory. This ensures you only see relevant snippets for the file you are editing.

#### Example Snippet Prefixes & Where They Work

- `appRouteNotFound` – Only in `**/app/**/not-found.tsx`
- `appRouteUnauthorized` – Only in `**/app/**/unauthorized.tsx`
- `appRouteForbidden` – Only in `**/app/**/forbidden.tsx`
- `appRouteError` – Only in `**/app/**/error.tsx`
- `appRouteLoading` – Only in `**/app/**/loading.tsx`
- `appRoutePage` – In `**/app/**/page.tsx` (standard or dynamic)
- `appRouteSearchPage` – In `**/app/**/page.tsx` or dynamic page files
- `appRouteLayout` – Only in `**/app/**/layout.tsx`
- `appRouteMetadata` – In `**/app/**/page.tsx` or `layout.tsx`
- `appRouteStaticParams` – In dynamic segment files like `[slug]/page.tsx`, `[slug]/layout.tsx`, or `[slug]/route.ts`

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

## Contributingdetailed guidelines on how to:
- Report bugs
- Request features
- Submit pull requests
- Follow code standards

## Support

- 📚 [Documentation](CONTRIBUTING.md)
- 🐛 [Report Issues](https://github.com/hedge-code/nextjs-app-router-snippets/issues)
- 💡 [Request Features](https://github.com/hedge-code/nextjs-app-router-snippets/issues)
- 📄 [View Changelog](CHANGELOG.md)

## License

This project is licensed under the [MIT License](LICENSE) – see the [LICENSE](LICENSE) file for details.

---

**Made with ❤️ for the Next.js community

**Enjoy faster Next.js development with App Router snippets!**
