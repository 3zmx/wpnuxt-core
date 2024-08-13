
This module is still being developed and not ready for production usage yet.
There will be many smaller alpha releases the coming weeks, often with breaking changes.

I am working towards a stable release. And will inform about it here

# WPNuxt

[![npm version][npm-version-src]][npm-version-href]
[![npm downloads][npm-downloads-src]][npm-downloads-href]
[![License][license-src]][license-href]
[![Nuxt][nuxt-src]][nuxt-href]

Nuxt module for using WordPress as a headless CMS with a Nuxt 3 frontend

- [✨ &nbsp;Release Notes](/CHANGELOG.md)
- [🏀 Online playground](https://stackblitz.com/github/wpnuxt/wpnuxt-core?file=playground%2Fapp%2Fpages%2Findex.vue)
- [📖 &nbsp;Documentation](https://wpnuxt.com)

## Features

- Content is fetched from WordPress using server-side GraphQL api calls
- Support for (Gutenberg Blocks) by adding the separate [@wpnuxt/blocks](https://github.com/wpnuxt/wpnuxt-blocks), which uses WPEngine's [wp-graphql-content-blocks](https://faustjs.org/tutorial/get-started-with-wp-graphql-content-blocks) and a set of custom vue components

## Quick Setup

Install the module to your Nuxt application with one command:

```bash
npx nuxi module add @wpnuxt/core
```

And connect WPNuxt to your wordpress installation in your nuxt.config.ts:

```json
wpNuxt: {
    wordpressUrl: 'https://yourwordpress.domain.com'
},
```

That's it! You can now use the WPNuxt module in your Nuxt app ✨

## Development

```bash
# Install dependencies
pnpm install

# Generate type stubs
pnpm run dev:prepare

# Develop with the playground
pnpm run dev

# Build the playground
pnpm run dev:build

# Run ESLint
pnpm run lint

# Run Vitest
pnpm run test
pnpm run test:watch

# Release new version
pnpm run release
```

<!-- Badges -->
[npm-version-src]: https://img.shields.io/npm/v/@vernaillen/wpnuxt/latest.svg?style=flat&colorA=18181B&colorB=28CF8D
[npm-version-href]: https://www.npmjs.com/package/@vernaillen/wpnuxt

[npm-downloads-src]: https://img.shields.io/npm/dm/@vernaillen/wpnuxt.svg?style=flat&colorA=18181B&colorB=28CF8D
[npm-downloads-href]: https://www.npmjs.com/package/@vernaillen/wpnuxt

[license-src]: https://img.shields.io/npm/l/@vernaillen/wpnuxt?style=flat&colorA=18181B&colorB=28CF8D
[license-href]: https://www.npmjs.com/package/@vernaillen/wpnuxt

[nuxt-src]: https://img.shields.io/badge/Nuxt-18181B?logo=nuxt.js
[nuxt-href]: https://nuxt.com
