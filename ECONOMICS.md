# Economics

IDART FUN treats **market economics** as a separate creator-facing choice from the market's launch profile.

The goal is to let creators choose not only how a market launches, but also how trading-fee economics are allocated across Creator, Holder Allocation and Protocol.

---

## Trading Fee

The current public product uses a fixed total trading fee reference of:

**2.50%**

The selected Economics mode changes the allocation model rather than the headline trading-fee rate.

---

## Economics Modes

| Economics Mode | Creator | Holder Allocation | Protocol |
|---|---:|---:|---:|
| **Creator First · Standard** | 60% | 10% | 30% |
| **All Win · Balanced** | 35% | 35% | 30% |
| **Holder Rewards · Community** | 10% | 60% | 30% |

---

## Creator First · Standard

Designed for launches that prioritize creator-side fee participation while preserving holder and protocol allocations.

**Allocation reference**

- Creator: `60%`
- Holder Allocation: `10%`
- Protocol: `30%`

---

## All Win · Balanced

Designed to create a more balanced split between creator participation, holder-oriented allocation and protocol economics.

**Allocation reference**

- Creator: `35%`
- Holder Allocation: `35%`
- Protocol: `30%`

---

## Holder Rewards · Community

Designed for communities that want a larger portion of protocol-side economics earmarked for future holder participation.

**Allocation reference**

- Creator: `10%`
- Holder Allocation: `60%`
- Protocol: `30%`

---

## Creator First Buy / Dev Buy

Creators may optionally participate in the launch transaction through a configurable Creator First Buy.

The product recalculates the applicable Meteora quote before signing so the creator can review the launch configuration and expected quote requirement before authorizing the transaction.

The Creator First Buy is a market-design option and is separate from the trading-fee allocation selected through Economics mode.

---

## Meteora Fee Accounting

Meteora DBC natively provides Creator / Partner fee accounting primitives.

IDART FUN builds its Economics layer around those primitives while maintaining a separate protocol-side model for holder allocations and future claim logic.

---

## Holder Allocation

Holder Allocation is a defined component of the IDART Economics model.

The planned Holder Rewards Router is intended to make this allocation transparent and claimable on a holder-by-holder basis through a dedicated protocol layer.

Until that router is live, the public product presents holder allocations as **defined market economics / earmarked protocol allocation**, rather than representing individual holder claims as already deployed.

---

## Economic Design Goal

IDART FUN is designed so that a Creator can combine:

```text
Market Profile
      +
Quote Asset
      +
Creator First Buy
      +
Economics Mode
      ↓
Configurable Launch Economics
```

This creates a market-design surface where launch behavior and fee economics can be configured independently.

---

## Multi-Asset Economic Opportunity

Because IDART FUN is designed to support SOL, USDC, compatible Solana tokens, xStocks and PreStocks as quote-market surfaces, Creators are not restricted to a single quote-asset universe.

This expands the design space for:

- market-specific demand;
- thematic market pairs;
- creator fee generation;
- holder-oriented economics;
- protocol revenue;
- stock / tokenized-asset market narratives;
- broader RWA-oriented market design.

IDART FUN does not represent any specific market configuration as a guarantee of liquidity, price appreciation or financial return.

---

# IDART FUN

## Design the Market. Launch the Asset.
