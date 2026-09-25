# IDART Fun Launchpad

**Design the market. Launch the asset.**

IDART Fun Launchpad is a Solana-native market-design launchpad built around **Meteora Dynamic Bonding Curve (DBC)**.

Rather than exposing creators to low-level market configuration, IDART turns configurable launch mechanics into a simple product flow: choose the asset, quote market, market profile, economics model, and graduation strategy.

## Live Demo

**https://launchpad.idartdex.xyz**

## Hackathon build

The public launch interface supports wallet connection, token/market configuration, quote-asset selection, market profiles, economics modes, and exportable launch configuration generation.

Direct browser-to-DBC transaction broadcast is still being integrated. However, the underlying Meteora DBC engine was validated **end-to-end on Solana Devnet** during the hackathon:

- real DBC config creation
- real token / virtual pool creation
- real DBC swaps
- separate creator and partner fee accrual
- graduation-safe final buy using `swapQuote2 + swap2 + SwapMode.PartialFill`
- 100% bonding-curve graduation
- successful migration to **Meteora DAMM v2**

## Interface

![IDART Launch Builder](screenshots/01-launch-builder.png)

The hackathon UI prepares and exports a structured Meteora DBC launch configuration and clearly distinguishes the browser configuration layer from the already-validated Devnet engine.

## End-to-end Devnet proof

### 1. Graduation reached safely

![100 percent graduation](screenshots/02-graduation-100.png)

The final DBC state reached:

- Quote reserve: `200000001` quote base units
- Migration threshold: `200000000` quote base units
- Graduation: `100.00%`
- Creator fees unclaimed: `931108` quote base units
- Partner fees unclaimed: `931108` quote base units

This demonstrates that the final purchase did **not** need to match the remaining threshold exactly. IDART's graduation-safe swap path used Meteora `PartialFill`, allowing the buy to consume only the remaining curve capacity.

### 2. DAMM v2 migration

![DAMM v2 migration](screenshots/03-damm-v2-migration.png)

After graduation, the DBC pool was successfully migrated to Meteora DAMM v2.

### 3. Final migrated state

![Migrated status](screenshots/04-migrated-status.png)

Final status confirmed:

- `Graduation: 100.00%`
- `Migrated: yes`
- creator and partner fees remained accounted for

## On-chain Devnet identifiers

- **Base Mint:** `8B1cJpMukfEbK5wJYixSnkpn5eGZWPpmtrRVPbYtPXZz`
- **DBC Pool:** `DYi5X52fshUZ3fYnex8Jbs1usFS5vT9zTAC4Tz4ooYEA`
- **DBC Config:** `DpLXcMud36KpyC6dxZQrjHyJRetWeF3M3yf6TsR2T9sC`

### Devnet transactions

- **Create Config:** `5bHRDBH6eU39M9fTo6XKoFJpXpLsk54WyzU3YP9XwctEkbVU23YjSZ3Nri6ZpihsgSFdP4NYgvqVjrmo113EBxMc`
- **Create Pool:** `5pnrQCLxri2qhrZkJAb8KUEnFymtLEK53S2qzZiPKYQqJGXwF4fuzrH3meCZR2gvq5MEfqmsatcroMYj4p2fVnJv`
- **First Swap:** `5ovFiywgwuXbsZcJ3uVGLDLnkkbtXVsfYSNpDp5JYqFE7SKadUCqEcTfQGGgHZuePqDGiSQjAPotCavKX4sKQeEr`
- **Graduation-safe PartialFill Swap:** `r8Vvmoi6g2CVJbsoEJJ76d7rNFefa4q751gr3ifLJyWuR2Toy4StftkvT4rqYrJZsbw2pyHDQ94MqTSHzUoqnvm`

## What makes IDART different

IDART combines:

- **Meteora DBC market design**
- **Multiple quote-asset choices**
- **Stock-paired markets using xStocks**
- **PreStocks market-pairing support**
- **Configurable market profiles**
- **Flexible economics models**
- **Creator / holder / platform incentive design**
- **DAMM v2 graduation**
- **Graduation-safe PartialFill trading**

The goal is not only to launch a token, but to let the creator define **how its market launches and how its economics are structured**.

## Market Profiles

- **Equity Quote** — designed for stock-token quote markets
- **Discovery** — designed for early price discovery
- **Balanced** — a general-purpose configuration

## Economics Modes

- **Creator First**
- **All-Win**
- **Holder Rewards**

Meteora DBC provides the native creator/partner fee-sharing layer. IDART's Holder Rewards mechanism is designed as an additional rewards-vault layer and remains a roadmap component until fully deployed.

## Quote Markets

- SOL
- USDC
- xStocks / tokenized public equities
- PreStocks / pre-IPO market assets
- compatible Solana tokens

Examples:

`Creator Token / TSLAx`

`Creator Token / OPENAI PreStocks`

## Lifecycle

`Create → Design Market → Meteora DBC → Trade → Bonding Progress → DAMM v2`

## Stocklana

IDART Fun Launchpad was built for **Stocklana 2026** with a focus on:

- **Main Track**
- **Meteora — Best Use of DBC**
- **PreStocks — Best Use of PreStocks**

## Architecture

- [Architecture Overview](docs/ARCHITECTURE.md)
- [Market Design](docs/MARKET_DESIGN.md)
- [Economics](docs/ECONOMICS.md)
- [Submission Snapshot](docs/SUBMISSION_SNAPSHOT.md)
- [Roadmap](docs/ROADMAP.md)

Implementation details, proprietary application code, deployment secrets, fee-routing logic, and internal market-configuration algorithms are intentionally not published in this showcase repository.

## Security

- No seed phrase should ever be requested.
- Private keys are never published in this repository.
- Wallet users approve their own transactions.
- Mainnet launches should be simulated and validated before broadcast.

## Links

- Launchpad: https://launchpad.idartdex.xyz
- IDARTDEX: https://idartdex.xyz
- X: https://x.com/IDARTDex_Coin
- Telegram: https://t.me/IDARTCoin

---

© 2026 IDARTDEX. All rights reserved.
