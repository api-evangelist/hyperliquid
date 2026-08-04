# Hyperliquid (hyperliquid)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Hyperliquid is a high-performance Layer 1 blockchain (HyperBFT consensus, HyperCore + HyperEVM execution) best known for its native perpetual futures and spot DEX with capacity for hundreds of thousands of orders per second. Developers and traders interact with Hyperliquid through a public REST and WebSocket API at api.hyperliquid.xyz for trading, order management, market data, and account state. Official Python and Rust SDKs wrap the API, and the node, order-book server, and HyperEVM tooling are open-sourced under the hyperliquid-dex GitHub organization.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/hyperliquid/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/hyperliquid/refs/heads/main/apis.yml)

## Tags

- DeFi
- Perpetuals
- DEX
- Layer 1
- Trading
- Order Book
- HyperEVM

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-29

## APIs

### Hyperliquid REST API

Public REST API for the Hyperliquid exchange. Read endpoints expose market metadata, order books, candles, trades, funding rates, user state, open orders, fills, and historical data. Write endpoints (under /exchange) accept signed actions for placing, cancelling, and modifying orders, transferring USDC, adjusting leverage, and managing sub-accounts and vaults.

- **Human URL:** [https://hyperliquid.gitbook.io/hyperliquid-docs/for-developers/api](https://hyperliquid.gitbook.io/hyperliquid-docs/for-developers/api)
- **Base URL:** `https://api.hyperliquid.xyz`

#### Tags

- REST
- Trading
- Market Data
- Perpetuals

#### Properties

- [Documentation](https://hyperliquid.gitbook.io/hyperliquid-docs/for-developers/api)
- [Postman Collection](collections/hyperliquid.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hyperliquid.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hyperliquid WebSocket API

Real-time WebSocket feed delivering order-book deltas, trades, candles, BBO, user fills, user funding, user-events, and active asset context. Also supports WebSocket-based POST actions for low-latency order management.

- **Human URL:** [https://hyperliquid.gitbook.io/hyperliquid-docs/for-developers/api/websocket](https://hyperliquid.gitbook.io/hyperliquid-docs/for-developers/api/websocket)
- **Base URL:** `wss://api.hyperliquid.xyz/ws`

#### Tags

- WebSocket
- Streaming
- Order Book
- Real-Time

#### Properties

- [Documentation](https://hyperliquid.gitbook.io/hyperliquid-docs/for-developers/api/websocket)
- [AsyncAPI](https://raw.githubusercontent.com/api-evangelist/hyperliquid/refs/heads/main/asyncapi/hyperliquid-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/hyperliquid.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hyperliquid.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hyperliquid Python SDK

Official Python SDK for the Hyperliquid REST and WebSocket APIs. Handles EIP-712 signing, action serialization, websocket subscription management, and typed wrappers for market and trading endpoints.

- **Human URL:** [https://github.com/hyperliquid-dex/hyperliquid-python-sdk](https://github.com/hyperliquid-dex/hyperliquid-python-sdk)
- **Base URL:** `https://github.com/hyperliquid-dex/hyperliquid-python-sdk`

#### Tags

- SDK
- Python
- Trading

#### Properties

- [Documentation](https://github.com/hyperliquid-dex/hyperliquid-python-sdk)
- [Repository](https://github.com/hyperliquid-dex/hyperliquid-python-sdk)
- [Postman Collection](collections/hyperliquid.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hyperliquid.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hyperliquid Rust SDK

Official Rust SDK for the Hyperliquid REST and WebSocket APIs, suited for high-performance market-making and trading clients.

- **Human URL:** [https://github.com/hyperliquid-dex/hyperliquid-rust-sdk](https://github.com/hyperliquid-dex/hyperliquid-rust-sdk)
- **Base URL:** `https://github.com/hyperliquid-dex/hyperliquid-rust-sdk`

#### Tags

- SDK
- Rust
- Trading

#### Properties

- [Documentation](https://github.com/hyperliquid-dex/hyperliquid-rust-sdk)
- [Repository](https://github.com/hyperliquid-dex/hyperliquid-rust-sdk)
- [Postman Collection](collections/hyperliquid.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hyperliquid.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Hyperliquid Node

Open-source Hyperliquid validator / non-validating node distribution used to participate in the HyperBFT consensus network and serve HyperCore + HyperEVM state.

- **Human URL:** [https://github.com/hyperliquid-dex/node](https://github.com/hyperliquid-dex/node)
- **Base URL:** `https://github.com/hyperliquid-dex/node`

#### Tags

- Node
- Validator
- Infrastructure

#### Properties

- [Documentation](https://github.com/hyperliquid-dex/node)
- [Repository](https://github.com/hyperliquid-dex/node)
- [Postman Collection](collections/hyperliquid.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hyperliquid.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### HyperEVM JSON-RPC

EVM-compatible JSON-RPC endpoint exposed by Hyperliquid for deploying and interacting with smart contracts on HyperEVM (chain ID 999), executed alongside HyperCore.

- **Human URL:** [https://hyperliquid.gitbook.io/hyperliquid-docs/hyperevm](https://hyperliquid.gitbook.io/hyperliquid-docs/hyperevm)
- **Base URL:** `https://rpc.hyperliquid.xyz/evm`

#### Tags

- JSON-RPC
- EVM
- HyperEVM
- Smart Contracts

#### Properties

- [Documentation](https://hyperliquid.gitbook.io/hyperliquid-docs/hyperevm)
- [Postman Collection](collections/hyperliquid.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/hyperliquid.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://hyperliquid.xyz)
- [Foundation](https://hyperfoundation.org)
- [Documentation](https://hyperliquid.gitbook.io/hyperliquid-docs)
- [Git Hub](https://github.com/hyperliquid-dex)
- [App](https://app.hyperliquid.xyz)
- [Stats](https://stats.hyperliquid.xyz)
- [Twitter](https://x.com/HyperliquidX)
- [Discord](https://discord.gg/hyperliquid)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
