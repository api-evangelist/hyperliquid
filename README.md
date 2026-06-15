# Hyperliquid (hyperliquid)

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
