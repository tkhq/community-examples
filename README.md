# Turnkey Community Examples

A community-maintained collection of integration guides showing how to use [Turnkey](https://turnkey.com) with popular protocols, frameworks, and ecosystems. Merged examples are published to [docs.turnkey.com](https://docs.turnkey.com).

---

## Contributing to Turnkey Community Examples

### Guidelines

- **Clear and focused** - A reader can follow it plainly, and understand the integration end to end
- **Uses Turnkey meaningfully** - The Turnkey integration is clear alongside your own product
- **Includes working code** - Code snippets should be accurate and generally working. Make sure any additional packages/dependencies are made clear for your example.

Follow the conventions established in the [Turnkey Cookbook](https://docs.turnkey.com/cookbook) as a guide for structure, depth, and quality when writing your example.

### Pull Request Template

You may copy [examples/template.mdx](./examples/template.mdx) as your starting point. See [examples/README.md](./examples/README.md) for full details on structure and conventions.

### PR checklist

Before opening a PR, confirm:

- [ ] File is at `examples/your-integration-name.mdx`
- [ ] Frontmatter includes `title` and `sidebarTitle`
- [ ] All five content sections are present and filled in
- [ ] No real API keys, org IDs, or wallet addresses are in the file
- [ ] Code snippets are accurate and follow the guidelines above
- [ ] Community Examples table (in this README) is updated with your example

### Review process

PRs are reviewed by the Turnkey team. We may ask for changes if:

- The MDX doesn't render correctly
- Sensitive values are present in code snippets
- The guide is missing key sections or hard to follow
- The Turnkey integration is unclear or incomplete

We aim to review PRs within a few business days.

### Deployment

This repo is a submodule of the [tkhq/docs](https://github.com/tkhq/docs) repository, which powers [docs.turnkey.com](https://docs.turnkey.com). Merged examples are reviewed by the Turnkey team and published to the live docs.

---

## Community Examples

| Example | Description | Contributor |
|---------|-------------|-------------|
| [YO Protocol](./examples/yo-protocol.mdx) | Deposit and redeem from ERC-4626 yield vaults using Turnkey wallets | YO Protocol |

---

## Resources

- [Turnkey Docs](https://docs.turnkey.com)
- [Turnkey SDK](https://github.com/tkhq/sdk)
