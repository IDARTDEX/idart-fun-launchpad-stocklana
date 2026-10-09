# Architecture Overview

This document intentionally describes the architecture at a high level. It does **not** disclose proprietary implementation code, internal routing logic, private infrastructure, or unreleased market-configuration algorithms.

---

## Product Flow

```text
Creator
  ↓
IDART Launch UI
  ↓
Token + Quote Asset + Market Profile + Economics
  ↓
Market Configuration Layer
  ↓
Meteora Dynamic Bonding Curve
  ↓
Trading / Bonding Progress
  ↓
DAMM v2 Graduation
  ↓
Post-Graduation Liquidity / Routing
  ↓
IDART Market Registry / Indexer
  ↓
Discovery Markets
  ↓
Dynamic Market Detail (/token/<mint>)
  ↓
Market Data + Trading + Metadata + Fee / Reward Surfaces
```

---

## Product Layers

1. **Creator Interface**  
   Collects the creator's token metadata, quote asset, Market Profile, Economics mode, Creator First Buy and launch configuration.

2. **Market Design Layer**  
   Maps creator-friendly Market Profiles and Economics choices into the supported launch configuration.

3. **Quote Asset Layer**  
   Resolves SOL, USDC, compatible Solana tokens, Token-2022 assets, xStocks and PreStocks exposed through the IDART Quote Asset Registry.

4. **Economics Layer**  
   Maps the selected economics model into creator/partner fee allocation and the protocol-side accounting required for future holder rewards.

5. **Meteora DBC Execution Layer**  
   Provides the bonding-curve, quote-asset, fee and graduation primitives used by IDART FUN.

6. **Graduation Layer**  
   Tracks bonding completion and migration from Meteora DBC into DAMM v2.

7. **Market Registry / Indexer**  
   Stores and resolves IDART-originated market references for Discovery and market-detail experiences.

8. **Discovery Markets**  
   Presents public market cards, status filters, quote-asset filters, search, sorting and market-route visibility.

9. **Market Detail Experience**  
   Combines token metadata, launch configuration, Market Profile, Economics, migration state, market charting, trading access and public fee / claim-status surfaces.

10. **Builders Surface**  
    Planned API, SDK and embeddable interfaces for third-party products to consume IDART market discovery, launch preparation and transaction-building capabilities.

---

## Current Public Architecture Evidence

The current public product already demonstrates:

- browser-native Meteora DBC launch execution;
- Devnet and Mainnet validation archives;
- successful Mainnet DBC → DAMM v2 migration;
- Discovery Markets;
- a public token-market index at `/token/`;
- a Mainnet MEMET market-detail reference page;
- official GeckoTerminal market chart integration;
- Jupiter embedded trading integration;
- a Quote Asset Registry with **1,274+ xStocks** and **8 PreStocks** surfaced;
- Token-2022 / TokenBadge-aware compatibility inspection;
- zero-cost Mainnet compatibility simulation using **AAPLx** as the representative xStock quote asset.

---

## Multi-Asset Quote Architecture

```text
Quote Asset Selection
        ↓
SOL / USDC / Solana Token / Token-2022 / xStock / PreStock
        ↓
Quote Asset Registry
        ↓
Metadata + Mint Program + Extensions + TokenBadge Inspection
        ↓
Supported IDART Launch Path
        ↓
Meteora DBC
```

The registry allows IDART FUN to move beyond a single fixed quote pair and treat quote-asset choice as part of the market-design experience.

---

## Discovery & Dynamic Market Routing

The next automation step is:

```text
Confirmed IDART Launch
        ↓
Market Registration
        ↓
Discovery Markets
        ↓
/token/<mint>
        ↓
On-chain State + Public Metadata
        ↓
GeckoTerminal + Jupiter + IDART Economics / Fee Surfaces
```

The existing MEMET market-detail page is the reference implementation for this dynamic market-detail architecture.

---

## Proprietary Boundary

This public repo intentionally excludes:

- production source code;
- private SDK wrappers;
- deployment configuration;
- unreleased profile parameter tables;
- fee-routing implementation;
- rewards-vault implementation;
- API secrets;
- private infrastructure;
- internal indexing logic.

The public repository focuses on product architecture, validation evidence, market-design concepts and auditable public references without exposing proprietary implementation.
