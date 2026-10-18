# Dexra

Dexra answers the questions an AI agent should ask before it trades on Solana. Every check returns a verdict (`ok`, `caution`, `avoid` or `unknown`), the reasons behind it and the evidence.

- **Launches**: pump.fun, LetsBonk, Raydium LaunchLab, Meteora DBC and PumpSwap, with creator history and first-buyer funding.
- **Tokens**: real holders after merging linked wallets, holder changes, mint authorities and Token-2022 traps.
- **Wallets**: exchange or not, bot or human, launch PnL, sanctions links.
- **Pools**: depth, liquidity flow, LP return after impermanent loss, sandwich share, CLMM range stats.
- **Perps and swaps**: funding, open interest and execution cost across venues; price impact and MEV risk before a swap.

## Connect

```sh
npx -y @dexra-dev/mcp install
```

This adds Dexra to every MCP client it finds: Claude Code, Claude Desktop, Cursor, VS Code, Codex, Windsurf, Gemini CLI, Antigravity and Cline. Add `--key dxr_...` to use a subscription.

- MCP: `https://api.dexra.dev/mcp` (Streamable HTTP). Configs for every client: [dexra-dev/mcp](https://github.com/dexra-dev/mcp)
- REST and x402 catalog: `https://api.dexra.dev/.well-known/x402`
- Docs: https://dexra.dev/docs
- Track record: https://dexra.dev/accuracy

Free tools work without an account. Paid tools cost 0.005–0.03 USDC per call over [x402](https://x402.org), or come with a subscription: Pro, Scale and Business plans with daily credits, monthly or yearly, at https://dexra.dev.

## Packages

- [`@dexra-dev/mcp`](https://www.npmjs.com/package/@dexra-dev/mcp): add Dexra to Claude, Cursor, VS Code and other MCP clients
- [`@dexra-dev/client`](https://www.npmjs.com/package/@dexra-dev/client): TypeScript client
- [`@dexra-dev/plugin-elizaos`](https://www.npmjs.com/package/@dexra-dev/plugin-elizaos): ElizaOS plugin
- [`@dexra-dev/plugin-solana-agent-kit`](https://www.npmjs.com/package/@dexra-dev/plugin-solana-agent-kit): Solana Agent Kit plugin
