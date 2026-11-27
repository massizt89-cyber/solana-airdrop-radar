# Solana Airdrop Radar

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Made with HTML](https://img.shields.io/badge/Made%20with-HTML5-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen.svg)](https://massizt89-cyber.github.io/solana-airdrop-radar/)

A web dashboard that tracks Solana airdrop, testnet, and free-claim opportunities in one place — with deadlines, status, and **links to official sources only**.

🔗 **Live demo:** https://massizt89-cyber.github.io/solana-airdrop-radar/

## What it does

- Lists Solana opportunities in a single table: project, type (airdrop / testnet / free claim), deadline, status, and official link.
- Read-only wallet checker: paste a public Solana address to see its SOL balance, JUP / GRASS / DUSD token balances, and devnet balance — and which opportunities can be checked on-chain at all.
- No wallet connection, no sign-up, no tracking — just a curated list you can check in a minute.
- Every link points to the project official site. No referral links, no shortened URLs.

## How to use

1. Open the [live demo](https://massizt89-cyber.github.io/solana-airdrop-radar/).
2. Check the deadline and status of each opportunity.
3. Click through to the official site and verify there before claiming anything.
4. Optional: paste a Solana address in the wallet checker to see what that wallet already holds (read-only, nothing is signed).

No build step, no dependencies — open `index.html` in any browser and it works (the wallet checker needs internet to reach Solana's public RPC).

## Adding an opportunity

Opportunities are curated by hand in `index.html`. To add one, copy a `<tr>` row in the table and fill in:

| Field | Rule |
|---|---|
| Project | Official project name |
| Type | `Airdrop`, `Testnet`, or `Free claim` |
| Deadline | `YYYY-MM-DD`, from the official announcement |
| Status | `Open`, `Closing soon`, or `Ended` |
| Official link | The project official site only — never a repost, aggregator, or shortened link |

## Roadmap

- [x] Real curated entries (live since 27 Nov 2026 — Jupiter, Grass, StandX, KRAiN, Solana Faucet)
- [x] Read-only wallet checker — paste a Solana address, see which opportunities it already joined (needs JavaScript)
- [ ] Status filter (All / Open / Ending soon)

## Safety notes

- This dashboard never asks you to connect a wallet or share a seed phrase. Any site that does is a scam.
- Always verify on the project official site before claiming anything — deadlines and eligibility change.
- Nothing here is financial advice.

## Project structure

```
.
├── index.html   # the dashboard (single file, no build step)
├── README.md    # this file
└── LICENSE      # MIT
```

## License

MIT — see [LICENSE](LICENSE).
