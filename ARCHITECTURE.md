# Architecture Overview

This document intentionally describes the architecture at a high level. It does **not** disclose proprietary implementation code, internal routing logic, private infrastructure, or unreleased market-configuration algorithms.

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
```

## Product Layers

1. **Creator Interface** — collects market-design choices.
2. **Market Design Layer** — maps creator-friendly profiles into launch parameters.
3. **Economics Layer** — maps the selected economics model into creator/partner fee allocation and future holder-reward accounting.
4. **Meteora DBC** — provides the bonding-curve, fee, quote-asset, and graduation primitives.
5. **Market Registry** — indexes IDART-originated markets for Explore and individual Market pages.
6. **Market Experience** — token information, Market DNA, bonding progress, economics, migration state, and trading access.

## Proprietary Boundary

This public repo intentionally excludes production source code, private SDK wrappers, deployment configuration, profile parameter tables, fee-routing implementation, rewards-vault implementation, API secrets, and internal indexing logic.
