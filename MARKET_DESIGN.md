# Market Design

IDART FUN separates market design into simple creator-facing decisions.

The product thesis is that launching a token should not require every creator to understand low-level bonding-curve configuration. Instead, creators select understandable market-design choices that map into supported Meteora DBC launch parameters.

---

## Quote Asset

Creators can design markets using multiple quote-asset categories exposed by the product:

- **SOL**
- **USDC**
- compatible Solana SPL tokens
- compatible Token-2022 assets
- **1,274+ xStocks** discoverable through the current Quote Asset Registry
- **8 PreStocks** integrated into the quote catalog

Quote-asset choice is part of the market design, not only a technical implementation detail.

---

## Market Profile

A Market Profile answers:

**How should this market launch and progress toward graduation?**

Current public Market Profiles:

| Market Profile | Starting MC | Graduation MC |
|---|---:|---:|
| **⚡ Lightning** | 28 SOL | 300 SOL |
| **⚖️ Smooth Graduation** | 35 SOL | 350 SOL |
| **📈 Scale Up** | 40 SOL | 450 SOL |

These are launch-configuration reference parameters and are not guarantees of market value, liquidity or future performance.

---

## Economics Mode

Economics answers:

**How should the market's trading-fee economics be allocated?**

Current product modes:

- **Creator First · Standard** — `60 / 10 / 30`
- **All Win · Balanced** — `35 / 35 / 30`
- **Holder Rewards · Community** — `10 / 60 / 30`

The three values represent Creator / Holder Allocation / Protocol.

---

## Creator First Buy

Creators can optionally participate in the launch transaction using a configurable Creator First Buy.

The product recalculates the applicable Meteora quote before signing so the creator can review the launch economics before authorizing the transaction.

---

## Graduation

IDART FUN is designed around the lifecycle:

```text
Create
  ↓
Meteora DBC
  ↓
Trading / Bonding
  ↓
100% Bonding
  ↓
DAMM v2 Graduation
```

This lifecycle has been validated end-to-end on both Solana Devnet and Mainnet using SOL as the quote asset.

---

## Multi-Asset Quote Markets

IDART FUN extends the market-design concept beyond a single SOL pair.

The public Quote Asset Registry currently surfaces:

- SOL
- USDC
- compatible Solana-token routes
- 1,274+ xStocks
- 8 PreStocks

The xStock quote-market path has also been validated against real Solana Mainnet state using **AAPLx** as the representative Token-2022 / stock-quote asset, including Meteora TokenBadge resolution, IDART DBC configuration simulation and fresh pool-creation simulation.

This allows IDART FUN to position quote-asset selection as part of the creator's market-design strategy.

---

## Market DNA

Each market is designed to expose a clear Market DNA:

- token / base asset
- quote asset
- Market Profile
- Economics mode
- total trading-fee model
- Creator / Holder Allocation / Protocol split
- Creator First Buy configuration
- bonding / graduation path
- migration state
- market metadata
- market links
- Discovery status

---

## Discovery & Market Detail

The public product now includes Discovery Markets and a Mainnet MEMET market-detail reference page.

The next automation step is:

```text
Confirmed Launch
      ↓
Automatic Market Registration
      ↓
Discovery Markets
      ↓
Dynamic /token/<mint>
```

This is intended to make every IDART-originated launch discoverable through the same product experience without requiring a manually created page for each market.

---

# IDART FUN

## Design the Market. Launch the Asset.
