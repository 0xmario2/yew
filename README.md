# YEW Agent Kit

**Your AI agent, on Robinhood Chain. Connect once. Access everything.**

YEW Agent Kit connects the AI assistant you already use — Claude Code, Codex, Cursor, Gemini CLI or Grok — to Robinhood Chain. One local MCP connection gives your agent **36 projects and 776 tools**: trade, lend, borrow, use vaults, bridge, and launch and trade tokens, all from a wallet that lives on your computer.

Robin Hood's longbow was carved from yew — the tree that bends and does not break. YEW is built the same way: one strong connection, rooted in Sherwood, reaching every project on the chain.

## Install

Use Node.js 22.12.0 or newer. In your terminal:

```bash
npm install -g @yewagentkit/addon
```

Then connect your assistant:

```bash
yew connect claude    # Claude Code
yew connect codex     # Codex
yew connect cursor    # Cursor (run from your project folder)
yew connect gemini    # Gemini CLI
yew connect grok      # Grok
```

Restart your app afterwards. Your wallet is created automatically on first use — your private key never leaves your computer, and YEW cannot recover a lost key.

### Claude Code plugin

Inside Claude Code:

```
/plugin marketplace add 0xmario2/yew
/plugin install yew@yew-agent-kit
```

### No-install shortcuts

The connect shortcuts run `npx -y @yewagentkit/addon@0.3.12 mcp` — no global install needed. One-click MCP install buttons for Cursor and VS Code are on the [website](https://yewagentkit.xyz).

## Your first prompts

- "Call account, balances and positions. Show my network, balances and setup status in plain English. Do not send any transactions."
- "Quote a swap of 5 USDG to ETH with the best route. Show the preview and do not swap yet."
- "Deposit 10 USDG into a Steakhouse vault. Show me the preview first."
- "What can you do with YEW? Group the tools by project."

Every action shows a plain summary first, then asks for your yes or no in chat. Approvals match the exact amount, never unlimited.

## How it works

- **Your computer** — the wallet is created locally and signs locally. Keys never leave the machine.
- **The YEW server** — prepares unsigned work only. It never sees your key and never signs or sends a transaction.
- **Robinhood Chain (mainnet 4663)** — swaps and deposits go straight from your wallet to the project.

Reads, quotes and previews are free and never sign anything. Actions need a verified ERC-8004 agent ID and your yes in chat. You can set an optional daily spending limit and change it any time by asking.

## Fees

YEW has no subscription. A 0.25% fee applies on swaps and bridges (including direct Uniswap and stock-token swaps; **no fee on FOBO, Pons and Hookr trades**), plain sends (added on top) and Morpho bundle actions, plus partner referral fees. Every fee is shown in the summary before you say yes.

**25% of YEW's income buys back and burns $YEW.** Holding $YEW has no access perks.

## $YEW

$YEW is launching soon on Robinhood Chain, live on [Pons](https://ponsfamily.com). The official contract address will be published on [yewagentkit.xyz](https://yewagentkit.xyz) first, at launch — any other address is not ours.

## Links

- Website: https://yewagentkit.xyz
- X: https://x.com/YewAgentKit
- Changelog: [CHANGELOG.md](CHANGELOG.md)

## License

Docs, examples and contracts are MIT. The compiled npm packages are Free-to-Use, No Copying; their source and the hosted YEW service are private.

YEW Agent Kit is independent software, not affiliated with Robinhood. Not financial advice. Nothing here is a promise about token prices or investment outcomes.
