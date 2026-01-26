# Contributing

Thank you for your interest in contributing to the LibreMatch Documentation!

## Ways to Contribute

### Reporting Issues

If you find errors, outdated information, or missing documentation:

1. Check if an [issue already exists](https://github.com/librematch/librematch-docs/issues)
2. If not, [open a new issue](https://github.com/librematch/librematch-docs/issues/new) with:
   - A clear description of the problem
   - The page/section affected
   - Suggested fix (if you have one)

### Improving Documentation

1. Fork the repository
2. Create a feature branch (`git checkout -b fix/typo-in-leaderboard`)
3. Make your changes
4. Test locally with `mdbook serve`
5. Submit a pull request

### Adding New Endpoint Documentation

When documenting a new API endpoint, please include:

- **HTTP method and path** as the title
- **Authentication requirements** (if any)
- **Request parameters** table with type and description
- **Example request** (with working URL if public endpoint)
- **Example response** with JSON
- **JSON Schema** (optional but helpful)

## Local Development

### Prerequisites

- [mdBook](https://rust-lang.github.io/mdBook/) - Install with `cargo install mdbook`

### Building

```bash
# Build the book
mdbook build

# Serve locally with hot-reload
mdbook serve
```

The book will be available at `http://localhost:3000`.

### Formatting

We use [dprint](https://dprint.dev/) for consistent formatting:

```bash
# Install dprint
cargo install dprint

# Check formatting
dprint check

# Auto-fix formatting
dprint fmt
```

## Style Guide

- Use ATX-style headers (`#`, `##`, etc.)
- Use fenced code blocks with language identifiers (`json,`bash, etc.)
- Keep lines under 80 characters where practical
- Use tables for parameter documentation
- Include working example URLs for public endpoints

## Pull Request Guidelines

- Keep PRs focused on a single change
- Update the `SUMMARY.md` if adding new pages
- Ensure `mdbook build` succeeds without errors
- Write clear commit messages

## Community

- [LibreMatch Discord](https://discord.gg/MvuusBxtuB)
- [GitHub Discussions](https://github.com/librematch/librematch-docs/discussions)

## License

By contributing, you agree that your contributions will be licensed under the [GNU Free Documentation License 1.3](./LICENSE).
