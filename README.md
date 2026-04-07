# CoinLog.ai — Your Crypto Data Stays on Your Infrastructure

Ask questions about your portfolio in plain language. The AI runs on your infrastructure, using your API keys. Your wallet addresses and balances never touch a third-party server.

**Live public test instance:** https://coinlog-ai.casey-digennaro.workers.dev

## Why This Exists
Most portfolio tools require you to send your wallet addresses to a remote server. This is built so you don't have to. You can ask "how much did my SOL gain this week?" without trusting an external privacy policy.

## Quick Start
1.  **Fork** this repository.
2.  **Deploy** to Cloudflare Workers with `wrangler deploy`.
3.  **Add your keys** for market data (CoinGecko) and an LLM (OpenAI).

Your instance is now live. No accounts, no databases, no hidden steps.

## How It Works
This is a single, readable JavaScript file deployed as a Cloudflare Worker. It has zero npm dependencies. You provide the API keys; the entire application logic runs within your isolated Cloudflare environment. No data is written to disk or logged.

## What You Can Do
*   **Self-Hosted Control**: Runs on Cloudflare Workers. Your portfolio data is queried live and never leaves your environment.
*   **Connect Wallets**: Supports EVM-compatible wallets via read-only RPC calls.
*   **Natural Language Queries**: Ask questions like "show me my worst performers this month" or "what's my total ETH balance?"
*   **Basic DeFi Overview**: See liquidity provider positions and unclaimed rewards for supported protocols.
*   **Fleet-Compatible**: Can be used standalone or connected to other agents in the Cocapn Fleet.

## Limitations
The agent provides a basic overview. Complex DeFi positions (e.g., nested yield strategies) may not be fully parsed. It currently supports EVM-compatible wallets only.

## License
MIT License. Fork-first open source.

---

<div style="text-align:center;padding:16px;color:#64748b;font-size:.8rem"><a href="https://the-fleet.casey-digennaro.workers.dev" style="color:#64748b">The Fleet</a> &middot; <a href="https://cocapn.ai" style="color:#64748b">Cocapn</a></div>