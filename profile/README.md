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

This adds Dexra to every MCP client it finds: Claude Code, Claude Desktop, Cursor, VS Code, Codex, Zed, OpenCode, GitHub Copilot CLI, Windsurf, Gemini CLI, Antigravity, Cline, Kiro, Amp, Qwen Code, Factory Droid and Augment. Add `--key dxr_...` to use a subscription.

- MCP: `https://api.dexra.dev/mcp` (Streamable HTTP). Configs for every client: [dexra-dev/mcp](https://github.com/dexra-dev/mcp)
- REST and x402 catalog: `https://api.dexra.dev/.well-known/x402`
- Docs: https://dexra.dev/docs
- Track record: https://dexra.dev/accuracy

Free tools work without an account. Paid tools cost 0.005–0.03 USDC per call over [x402](https://x402.org), or come with a subscription: Pro, Scale and Business plans with daily credits, monthly or yearly, at https://dexra.dev.

## Agent templates

Agents that trade on Solana and ask Dexra before every buy. Each is a GitHub template, runs as a dry run until you turn live trading on, and trades through the Jupiter Swap API. Guide: https://dexra.dev/docs/templates

| Template | Framework |
|---|---|
| [template-elizaos](https://github.com/dexra-dev/template-elizaos) | elizaOS |
| [template-hermes](https://github.com/dexra-dev/template-hermes) | Hermes Agent (skill + MCP server) |
| [template-solana-agent-kit](https://github.com/dexra-dev/template-solana-agent-kit) | Solana Agent Kit |
| [template-vercel-ai-sdk](https://github.com/dexra-dev/template-vercel-ai-sdk) | Vercel AI SDK |
| [template-claude-agent-sdk](https://github.com/dexra-dev/template-claude-agent-sdk) | Claude Agent SDK |
| [template-openai-agents](https://github.com/dexra-dev/template-openai-agents) | OpenAI Agents SDK (Python) |
| [template-langgraph](https://github.com/dexra-dev/template-langgraph) | LangGraph (Python) |
| [template-launch-bot](https://github.com/dexra-dev/template-launch-bot) | No LLM: a launch bot |

## Packages

- [`@dexra-dev/mcp`](https://www.npmjs.com/package/@dexra-dev/mcp): add Dexra to Claude, Cursor, VS Code and other MCP clients
- [`@dexra-dev/client`](https://www.npmjs.com/package/@dexra-dev/client): TypeScript client
- [`@dexra-dev/plugin-elizaos`](https://www.npmjs.com/package/@dexra-dev/plugin-elizaos): ElizaOS plugin
- [`@dexra-dev/plugin-solana-agent-kit`](https://www.npmjs.com/package/@dexra-dev/plugin-solana-agent-kit): Solana Agent Kit plugin
