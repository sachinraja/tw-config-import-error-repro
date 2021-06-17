# TailwindCSS Config Import Error Repro


I get the following error when importing `tailwindcss/resolveConfig`. The error occurs when Next.js attempts to compile a page. The import is in `pages/index.js`.
```
(node:155489) [DEP_WEBPACK_MODULE_ISSUER] DeprecationWarning: Module.issuer: Use new ModuleGraph API

error - ./node_modules/modern-normalize/modern-normalize.css
Global CSS cannot be imported from within node_modules.
Read more: https://nextjs.org/docs/messages/css-npm
Location: node_modules/tailwindcss/lib/plugins/preflight.js
Could not find files for / in .next/build-manifest.json
```

To reproduce run
  1. `npm i`
  2. `npm run dev`
