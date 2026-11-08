# Portfolio 2.0 — Quality checks

The new `Portfolio quality checks` GitHub Actions workflow runs **independently** of the existing Pages deployment workflow. No existing deployment configuration was modified.

## Run locally

Requires Node.js 22 or newer:

```sh
node --check assets/app.js
node --test tests/portfolio.test.cjs
```

## Coverage

- Required HTML elements and Persian RTL markup
- Exactly 10 distinct GitHub repository links
- Expected GitHub Pages demo URL structure
- Search and category filters
- Empty search state
- HTML escaping helper
- JavaScript syntax

Tests use Node's built-in test runner and a minimal DOM fixture. They do **not** replace browser-based end-to-end tests, visual checks, accessibility audits, or verification that remote GitHub Pages URLs respond successfully.

## Safety

This workflow only reads repository files and executes tests. It does not deploy, publish, write repository contents, access secrets, or modify any of the other nine projects.
