# CoinLog.ai — Self-Hosted Crypto Analysis Agent

You keep control of your portfolio data. CoinLog is a private agent you run yourself, designed to provide on-chain and market insights without sending your information to a third-party service.

**Live public instance (no sign-up):** https://coinlog-ai.casey-digennaro.workers.dev  
This is the exact code you will deploy. No user data is retained.

---

## Quick Start

Deploy your own private instance in a few minutes:
1.  Fork this repository.
2.  Deploy to Cloudflare Workers using `wrangler deploy`.
3.  Configure your own API keys as environment variables.

---

## How This Works

CoinLog is an agent runtime built for self-hosting. You provide the API keys for market data, LLM inference (like OpenAI or Anthropic), and read-only access to your wallets or exchanges. The agent runs on your Cloudflare Workers account and only makes calls to services you have explicitly configured.

**Core principle:** Your keys, your data, your infrastructure.

---

## Features

*   **Self-Hosted Control**: Runs on your Cloudflare account. Your portfolio data never leaves your setup.
*   **Portfolio Context**: Connect most EVM-compatible wallets or read-only exchange APIs you configure.
*   **Market Analysis**: Query your holdings with current market data using an LLM you control.
*   **DeFi Position Overview**: Review basic liquidity pool positions and rewards.
*   **Zero Runtime Dependencies**: Built for Cloudflare Workers; no npm dependencies.
*   **Fleet-Compatible**: Optionally interoperate with other agents in the Cocapn Fleet, or run standalone.

## One Honest Limitation

Setting up integrations requires manual API key configuration for each service (e.g., blockchain RPC, market data, LLM). This gives you full control but means initial setup is not a single-click process.

---

## License & Contribution

MIT Licensed. Use, modify, and redistribute for any purpose.

This is an open agent in the Cocapn Fleet. The project follows a fork-first philosophy. You are encouraged to fork the repository and adapt it to your needs. Bug fixes and clear, minimal feature additions are welcome.

---

MIT License • Superinstance & Lucineer (DiGennaro et al.)

<div align="center">
  <a href="https://the-fleet.casey-digennaro.workers.dev">The Fleet</a> • <a href="https://cocapn.ai">Cocapn</a>
</div>