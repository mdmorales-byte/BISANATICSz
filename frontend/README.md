# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some Oxlint rules.

Currently, two official plugins are available:


## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the Oxlint configuration

If you are developing a production application, we recommend enabling type-aware lint rules by installing `oxlint-tsgolint` and editing `.oxlintrc.json`:

```json
{
  "$schema": "./node_modules/oxlint/configuration_schema.json",
  "plugins": ["react", "typescript", "oxc"],
  "options": {
    "typeAware": true
  },
  "rules": {
    "react/rules-of-hooks": "error",
    "react/only-export-components": ["warn", { "allowConstantExport": true }]
  }
}
```

See the [Oxlint rules documentation](https://oxc.rs/docs/guide/usage/linter/rules) for the full list of rules and categories.
# Mini Management System - Frontend

React, TypeScript, and Vite frontend for the Mini Management System prototype.

## Source layout

```text
src/
  assets/       Imported images and other bundled assets
  components/   Shared UI components
  pages/        Page-level views
  services/     API and external-service access
  types/        Shared TypeScript types
  utils/        Small reusable helpers
  App.tsx       Application root
  main.tsx      Browser entry point
```

Static files served without bundling belong in `public/`. Keep feature-specific code close to the feature as the application grows.

## Commands

Run these commands from the `frontend/` directory:

```sh
npm install
npm run dev
npm run build
npm run lint
npm run preview
```
