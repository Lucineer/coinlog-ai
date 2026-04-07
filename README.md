# CoinLog.ai — AI Crypto Companion

You check your wallets multiple times a day. You still don't have a clear narrative of your portfolio.

### Why this exists
Most crypto trackers lock your data inside their platform. This is an agent you own. It runs on your infrastructure and answers the questions you ask in plain English. No third party ever sees your holdings.

Built on Cloudflare Workers with zero dependencies. Part of the Cocapn Fleet.

**Live URL:** https://coinlog-ai.casey-digennaro.workers.dev

---

## What makes this different
- **You own the agent.** Fork this repository. It runs on your Cloudflare account. No one can shut it off.
- **No telemetry.** Your wallet addresses and queries never leave your worker.
- **One source file.** No build step or `node_modules`. Deploy in under two minutes.
- **Natural language interface.** Ask "what's my largest holding?" or "how much yield did I earn this week?"

---

## Features
- Track any wallet balance across EVM chains
- Pull market data from top exchanges
- View basic DeFi positions (supply, borrow, stake)
- Query your portfolio using natural language
- Optional Bring Your Own Key for AI and data providers
- Zero runtime dependencies; runs entirely on Cloudflare's edge
- Interoperable with other Cocapn Fleet agents

---

## Quick Start
1. Fork this repository.
2. Deploy it to Cloudflare Workers (no configuration needed).
3. Edit `worker.ts` to add your own keys or adjust the agent's behavior.

---

## Architecture
A single Cloudflare Worker that follows the Cocapn Fleet protocol. It exposes structured endpoints for portfolio queries and uses external APIs for market data. All logic executes at the edge, in your instance.

---

## Bring Your Own Keys
You control all external connections. Provide your own keys for:
- AI models (OpenAI, Anthropic, or compatible providers)
- Crypto market data APIs
- Blockchain RPC endpoints

Keys are only sent from your worker directly to the target service.

---

## Limitations
This runs on Cloudflare Workers, which imposes execution time and memory constraints. Complex portfolio analysis with hundreds of positions may hit these limits. The agent is designed for clarity, not high-frequency trading.

---

## Contributing
This is an open vessel in the Cocapn Fleet. Fork first, build what you need, and open a pull request when it's ready. For major changes, please open an issue to discuss.

---

## License
MIT License

Superinstance & Lucineer (DiGennaro et al.)

---

<div align="center">
  <a href="https://the-fleet.casey-digennaro.workers.dev">The Fleet</a> • 
  <a href="https://cocapn.ai">Cocapn</a>
</div>