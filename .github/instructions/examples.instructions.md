---
applyTo: "examples/**/*.mdx"
---

Review this file against the structure defined in [examples/template.mdx](../../examples/template.mdx) and the standards in [examples/README.md](../../examples/README.md).

## PR template standards

The file must follow the required MDX structure. Flag if:
- Frontmatter is missing `title` or `sidebarTitle`
- The `title` does not mention Turnkey and clearly describe the integration (exact phrasing is flexible - e.g. "Use Turnkey wallets with Jupiter", "Building on Yield.xyz with Turnkey", and "Builder Codes with Turnkey on Base" are all valid)
- The `sidebarTitle` is missing or overly long (keep it short for sidebar display)
- Any of the five required sections are missing or still contain unfilled placeholder content: Overview, Getting started, Install dependencies, integration steps, Summary

## Code standards

- Code blocks must use `tsx` for TypeScript/React and `bash` for shell commands
- No hardcoded secrets, private keys, wallet addresses, or real org IDs - only `process.env.VAR_NAME` or clearly labeled placeholder strings
- Code must reflect a real integration, not pseudocode
- Snippets should be focused on the relevant portion, not entire files

## Security

Flag as a blocking issue if any of the following are present:
- Code that exports, logs, or transmits private keys or seed phrases
- Transactions that send funds to a hardcoded external address without clear user intent
- Code that reads environment variables and sends them to an external endpoint
- HTTP requests to URLs outside of the stated protocol's official API

## Language and content

Flag if the file contains:
- Profanity, slurs, or offensive language
- Disparaging claims about Turnkey or other protocols
- Claims about Turnkey's security, reliability, or guarantees that go beyond what is documented at docs.turnkey.com
- Content unrelated to the stated integration
