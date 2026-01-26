# LibreMatch Documentation

[![Deploy mdBook](https://github.com/librematch/librematch-docs/actions/workflows/mdbook.yml/badge.svg)](https://github.com/librematch/librematch-docs/actions/workflows/mdbook.yml)
[![Check Links](https://github.com/librematch/librematch-docs/actions/workflows/url-check.yml/badge.svg)](https://github.com/librematch/librematch-docs/actions/workflows/url-check.yml)
[![License: GFDL 1.3](https://img.shields.io/badge/License-GFDL%201.3-blue.svg)](https://www.gnu.org/licenses/fdl-1.3.html)

Community-driven documentation for Age of Empires API endpoints and data sources.

**[Read the documentation](https://librematch.github.io/librematch-docs/)**

## What's Inside

- **WorldsEdgeLink API** - Documentation for the Relic Link / Worlds Edge Link API used by Age of Empires games
- **Age of Empires API** - Official ageofempires.com API endpoints
- **LibreMatch Design** - Architecture and design documentation for the LibreMatch project

## Building Locally

This documentation is built with [mdBook](https://rust-lang.github.io/mdBook/).

### Installation

```bash
# Install mdbook
cargo install mdbook

# Or download a release binary from:
# https://github.com/rust-lang/mdBook/releases
```

### Build & Serve

```bash
# Build static HTML to ./book
mdbook build

# Serve locally with hot-reload at http://localhost:3000
mdbook serve
```

## Contributing

Contributions are welcome! Please feel free to submit issues and pull requests.

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## Community

- [LibreMatch Discord](https://discord.gg/MvuusBxtuB)
- [GitHub Organization](https://github.com/librematch)

## License

This documentation is licensed under the [GNU Free Documentation License 1.3](./LICENSE).
