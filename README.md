# CoinLog.ai — Self-Hosted Crypto Portfolio Agent

You shouldn't have to send your wallet history and portfolio data to a third-party service just to understand what you own.

### Why it was built
Many portfolio trackers lock your data or treat their analysis as a black box. CoinLog is a self-hosted agent that gives you control. It runs on your own Cloudflare Worker—no middleman server ever handles your private keys or data.

This is a standard vessel on the Cocapn Fleet, built using open protocols for interoperability with other agents.

**Live test instance:** https://coinlog-ai.casey-digennaro.workers.dev

---

### How it works
- **Fully self-hosted** – You deploy and control the instance. No telemetry or mandatory accounts.
- **Fork-first** – Adapt the code for your needs, then share improvements back if you choose.
- **Zero runtime dependencies** – Every line that runs in production is visible in this repository.
- **BYOK (Bring Your Own Keys)** – The agent has no built-in backend keys. You supply all credentials via environment variables.

---

### What you can do
- **Track holdings** – View balances from connected EVM wallets and exchange APIs you configure.
- **Query with context** – Ask questions about your portfolio using an LLM, with access to current market data.
- **Basic DeFi context** – Review position data for supported liquidity pools.
- **Fleet-native** – Communicate with other agents in the Cocapn Fleet for expanded workflows.
- **MIT Licensed** – Use, modify, or distribute without restriction.

---

### Quick start
1. **Fork** this repository.
2. **Deploy** to Cloudflare Workers.
3. **Configure** your API keys in the worker environment variables.

---

### Bring Your Own Keys
You supply and control all external service keys. The agent supports:
- Market data APIs (CoinGecko, CoinMarketCap)
- LLM providers (OpenAI, Anthropic, or local models via a tunnel)
- Read-only wallet and exchange APIs

No keys are shared with or sent to Cocapn or Fleet infrastructure.

---

### One current limitation
The agent requires manual configuration of each data source and does not automatically discover or sync all possible DeFi positions. You set up the integrations you need.

---

### Contributing
This is a public Fleet vessel. Fork the repository, build what you need, and contributions back are welcome. Focus on bug fixes, reliability, and well-scoped features.

---

MIT License • Superinstance & Lucineer (DiGennaro et al.)

---

<div align="center">
  <a href="https://the-fleet.casey-digennaro.workers.dev">The Fleet</a> • <a href="https://cocapn.ai">Cocapn</a>
</div>