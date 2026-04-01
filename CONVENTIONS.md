# Community Examples Conventions

This file defines the standards every example in this repo must meet. It is used by automated PR review to evaluate submissions.

---

## File structure

- Each example is a single MDX file located at `examples/your-integration-name.mdx`
- File names should be lowercase, hyphen-separated, and descriptive (e.g. `jupiter-solana-swap.mdx`)

---

## Frontmatter

Every file must include both fields:

```mdx
---
title: 'Use Turnkey wallets with [Protocol]'
sidebarTitle: "[Protocol] integration"
---
```

- `title` must follow the pattern "Use Turnkey wallets with [Protocol]"
- `sidebarTitle` must follow the pattern "[Protocol] integration"

---

## Required sections

Every example must contain all five sections in this order:

1. **Overview** - what the protocol is and what the integration does
2. **Getting started** - prerequisites including Turnkey org setup and any external API keys or funded wallets required
3. **Install dependencies** - `npm install` command with all required packages listed
4. **Integration steps** - one or more sections covering the meaningful steps of the integration, each accompanied by a code snippet
5. **Summary** - a bullet list of what the reader learned

---

## Code standards

- Use `tsx` for TypeScript and React code blocks, `bash` for shell commands
- Code must be accurate and reflect a real, working integration - not pseudocode
- No hardcoded secrets, private keys, wallet addresses, or org IDs - use `process.env.VAR_NAME` or clearly labeled placeholder strings
- Snippets should be focused - show the relevant portion, not entire files

---

## Language standards

- Writing must be clear, professional, and technically accurate
- No profanity, inflammatory language, or content unrelated to the integration
- Protocol and package names should be spelled and capitalized correctly
- Do not make claims about Turnkey's security, reliability, or guarantees beyond what is documented at docs.turnkey.com

---

## Security - patterns to reject

Flag and reject any example that contains:

- Code that exports, logs, or transmits private keys or seed phrases
- Transactions that drain wallet balances to an external address without explicit user intent
- Code that reads and exfiltrates environment variables to an external endpoint
- Calls to unrecognized or suspicious external URLs outside of the stated protocol's official API
- Any pattern that could compromise a user's wallet or credentials

---

## README table

The root `README.md` Community Examples table must be updated with every new submission, including the example name, a short description, and the contributor's name or company.
