# Examples Overview

Each example is a single MDX file in this directory. These pages are rendered directly in the Turnkey docs site, so they follow the same conventions as the rest of the docs.

Copy the template as a starting point:

```bash
cp examples/template.mdx examples/your-integration-name.mdx
```

---

## Frontmatter

Every MDX file must include:

```mdx
---
title: 'Your integration title'
sidebarTitle: "Short sidebar label"
---
```

- `title` - shown in the page header and search results. Use `'Use Turnkey wallets with [Protocol]'` as a starting point, but other phrasings are fine as long as Turnkey and the integration are clearly described - e.g. "Building on Yield.xyz with Turnkey" or "Builder Codes with Turnkey on Base"
- `sidebarTitle` - shown in the docs sidebar, keep it short

---

## Content structure

1. **Overview** - what the protocol is and what the integration does
2. **Getting started** - prerequisites (Turnkey org setup, external API keys, funded wallets, etc.)
3. **Install dependencies** - `npm install` with relevant packages
4. **Integration steps** - one section per meaningful step, each with a code snippet
5. **Summary** - bullet list of what the reader learned

---

## Code guidelines

- Use `tsx` for TypeScript/React snippets, `bash` for shell commands
- Show real, accurate code - not pseudocode
- Don't hardcode real API keys, org IDs, or wallet addresses - use `process.env.YOUR_VAR` or placeholder strings
- Keep snippets focused - show the relevant part, not an entire file

---

## Linking to source code

If you have a full working repo for your example, link to it in the Overview section. This is encouraged but not required.
