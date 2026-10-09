# IDART FUN

### Design the Market. Launch the Asset.

**IDART FUN** is a Solana-native programmable market launchpad built on **Meteora Dynamic Bonding Curve (DBC)**.

Creators can configure how a market launches — including the token, quote asset, Market Profile, economics mode, creator first buy, bonding path and graduation to **Meteora DAMM v2**.

---

## 🌐 Live Product

- **Website:** https://idartfun.xyz
- **Launch:** https://idartfun.xyz/launch/
- **Discovery Markets:** https://idartfun.xyz/token/
- **Mainnet Market Detail (MEMET):** https://idartfun.xyz/token/memet/
- **API for Builders — Coming Soon:** https://idartfun.xyz/idart-api-for-builders/
- **X:** https://x.com/IDARTFun_Launch
- **Legacy Stocklana URL:** https://launchpad.idartdex.xyz  
  Redirects to the current IDART FUN domain.

> **Stocklana repository notice**
>
> This repository remains the public record of the **Stocklana 2026 submission**.
>
> The original submission state is preserved in [`SUBMISSION_SNAPSHOT.md`](./SUBMISSION_SNAPSHOT.md).
>
> Features completed after the deadline are clearly identified below as **Post-Submission Progress**.

---

# ✅ Post-Submission Progress — October 2026

Since the Stocklana submission, IDART FUN has progressed from its submitted MVP into a substantially more complete launchpad with a validated browser-native lifecycle and a broader multi-asset market layer.

## Core lifecycle now validated

- ✅ Solana Devnet end-to-end launch
- ✅ Solana Mainnet end-to-end launch with real SOL
- ✅ Meteora DBC config and pool creation
- ✅ Wallet-signed swaps
- ✅ Creator First Buy / Dev Buy
- ✅ Live bonding progress
- ✅ Graduation-safe `PartialFill`
- ✅ 100% bonding
- ✅ Successful **DBC → DAMM v2** migration
- ✅ Creator and partner fee accrual
- ✅ Existing-market recovery without recreating the token or pool
- ✅ Devnet and Mainnet validation archives in the Launch UI

## Product layer now available

- Configurable Market Profiles
- Configurable Economics modes
- Production Mainnet market-cap targets
- Public token metadata preparation
- Website and social metadata fields
- Launch Review before transaction signing
- Mandatory safety and risk acknowledgements
- Browser wallet integration
- Mainnet transaction simulation before approval
- Discovery Markets interface with market-status, quote-asset, search, sort and card/table views
- Public token-market index at `/token/`
- Mainnet MEMET market-detail page at `/token/memet/`
- Official GeckoTerminal market chart integration
- Jupiter embedded trading integration
- Quote Asset Registry with **1,274+ xStocks**
- **8 PreStocks** integrated into the quote-asset catalog
- Token-2022 / Transfer Hook compatibility inspection
- Mainnet xStock quote compatibility validation using real **AAPLx + Meteora TokenBadge**
- Zero-cost Mainnet RPC simulation diagnostics for quote-market compatibility
- API for Builders preview
- Responsive desktop, tablet and mobile UI

## In active development

- Automatic post-launch market registration in Discovery
- Dynamic market-detail routing for future `/token/<mint>` pages
- Holder Rewards Router and holder claims
- Extended compatibility validation across additional Token-2022 quote assets
- Builders API / SDK / low-code embeds
- Partner attribution and builder-originated transaction economics
- Address Lookup Table support where appropriate
- Additional wallet-security compatibility improvements

---

# 🚀 Verified Mainnet Lifecycle

IDART FUN completed and publicly verified a real Mainnet launch through the full market lifecycle:

`Create → Meteora DBC → Buy / Trade → 100% Bonding → DAMM v2`

## Mainnet validation market

| Field | Value |
|---|---|
| **Token** | Meme Tesla Club Test |
| **Symbol** | MEMET |
| **Network** | Solana Mainnet |
| **Base Mint** | `3qekQqW4YLLTjNPfaSB8AaQ9MUpTcthck4qKARM7uhSL` |
| **DBC Pool** | `2K1PYMVUChhBLPwfQ5ZAjgFwVTPXa34UKdGJkQwrrTFm` |
| **Final Bonding** | **100%** |
| **Migration** | **DAMM v2** |
| **Final State** | **Migrated** |

## Mainnet proof

- **Launch + Initial Buy TX**  
  https://explorer.solana.com/tx/5SPwDnURxJeANhUJawmb9Zb7cifBZcMnCgTtwgCwSTJ9Xy2Sz4MeYGgTp61QscAjxKLqEhriiCgEspbgm3jMPU4R

- **Base Mint**  
  https://explorer.solana.com/address/3qekQqW4YLLTjNPfaSB8AaQ9MUpTcthck4qKARM7uhSL

- **DBC Pool**  
  https://explorer.solana.com/address/2K1PYMVUChhBLPwfQ5ZAjgFwVTPXa34UKdGJkQwrrTFm

- **External Market View**  
  https://dexscreener.com/solana/2k1pymvuchhblpwfq5zajgfwvtpxa34ukdgjkqwrrtfm

- **DAMM v2 Migration TX**  
  https://solscan.io/tx/43BAGHCMeDpsgPyQSBZpXioBdQ6WmiHWfSvvz6waAiue3bjAsDC1oHFKPjuCvipedwvcsxV9kuTv7MCHQeSTUJZg

### Migration confirmation

- **Result:** SUCCESS
- **Status:** Finalized
- **Instruction:** `Migration_damm_v2`
- **Migration Target:** Meteora DAMM v2

The public Launch page also includes a **Verified Mainnet Validation Archive** so evaluators can inspect the completed lifecycle without initiating another Mainnet test.

---

# 🧪 Verified Devnet Lifecycle

The original Devnet validation remains part of the submission evidence.

## Devnet identifiers

| Field | Address |
|---|---|
| **Base Mint** | `8B1cJpMukfEbK5wJYixSnkpn5eGZWPpmtrRVPbYtPXZz` |
| **DBC Pool** | `DYi5X52fshUZ3fYnex8Jbs1usFS5vT9zTAC4Tz4ooYEA` |
| **DBC Config** | `DpLXcMud36KpyC6dxZQrjHyJRetWeF3M3yf6TsR2T9sC` |

## Devnet transactions

- **Create Config:** `5bHRDBH6eU39M9fTo6XKoFJpXpLsk54WyzU3YP9XwctEkbVU23YjSZ3Nri6ZpihsgSFdP4NYgvqVjrmo113EBxMc`
- **Create Pool:** `5pnrQCLxri2qhrZkJAb8KUEnFymtLEK53S2qzZiPKYQqJGXwF4fuzrH3meCZR2gvq5MEfqmsatcroMYj4p2fVnJv`
- **First Swap:** `5ovFiywgwuXbsZcJ3uVGLDLnkkbtXVsfYSNpDp5JYqFE7SKadUCqEcTfQGGgHZuePqDGiSQjAPotCavKX4sKQeEr`
- **Graduation-safe PartialFill:** `r8Vvmoi6g2CVJbsoEJJ76d7rNFefa4q751gr3ifLJyWuR2Toy4StftkvT4rqYrJZsbw2pyHDQ94MqTSHzUoqnvm`

### Devnet validation demonstrated

- Real DBC config creation
- Real token / virtual pool creation
- Real DBC swaps
- Creator / partner fee accrual
- Graduation-safe final buy using PartialFill
- 100% bonding
- Successful DAMM v2 migration

---

# 🧩 Market Design

IDART FUN is designed as a **market-design layer over Meteora**, not only a token generator.

## Market Profiles

| Profile | Starting MC | Graduation MC | Purpose |
|---|---:|---:|---|
| **⚡ Lightning** | 28 SOL | 300 SOL | Faster price discovery and lower initial market-cap path |
| **⚖️ Smooth Graduation** | 35 SOL | 350 SOL | Balanced general-purpose launch path |
| **📈 Scale Up** | 40 SOL | 450 SOL | Higher-capacity launch path |

> These are market-cap reference parameters used by the launch configuration. They are not guarantees of liquidity, price or future value.

---

# 💰 Economics Modes

The public design keeps the total trading fee fixed at **2.50%**, while the allocation logic changes by Economics mode.

| Economics Mode | Creator | Holder Allocation | Protocol |
|---|---:|---:|---:|
| **Creator First · Standard** | 60% | 10% | 30% |
| **All Win · Balanced** | 35% | 35% | 30% |
| **Holder Rewards · Community** | 10% | 60% | 30% |

Meteora DBC provides native **Creator / Partner** fee accounting.

IDART's holder-by-holder **Rewards Router** is a separate protocol layer and remains under active development. The public product does not claim holder claims are fully deployed until that router is live.

---

# 🪙 Creator First Buy / Dev Buy

Creators may optionally participate in the launch transaction with a first buy.

The production UI supports a configurable creator first-buy percentage and recalculates the exact Meteora quote before signing.

As a reference:

- **Lightning profile**
- **5% Creator First Buy**
- approximately **1.5 SOL**

The actual Meteora quote shown before wallet signing is authoritative.

---

# 📊 Quote Markets

IDART FUN is designed as a **multi-asset quote-market layer for Solana**.

Current public quote surfaces include:

- **SOL**
- **USDC**
- Compatible Solana SPL tokens
- Compatible Token-2022 assets
- **1,274+ xStocks** discoverable through the current Quote Asset Registry
- **8 PreStocks** integrated into the current quote-asset catalog

The Quote Asset Registry inspects public asset metadata and on-chain mint properties before exposing quote assets inside the launch interface.

## xStocks Mainnet compatibility validation

The xStock quote path has now been validated against real Solana Mainnet state using **AAPLx** as the representative Token-2022 / stock-quote asset.

Validation result:

- **AAPLx quote mint:** `XsbEhLAtcf6HdfpFZ5xEMdqW8nfAvcsP5bdudRLJzJp`
- **Meteora TokenBadge:** resolved successfully
- **IDART exact DBC config simulation:** PASS
- **Fresh AAPLx createPool builder:** PASS
- **Fresh AAPLx Mainnet simulation:** PASS
- **Units consumed:** `111031`
- **Diagnostic cost:** `0 SOL`
- **Wallet signature:** not requested
- **Broadcast:** none

This validation demonstrates that the IDART browser engine can resolve the real AAPLx Token-2022 mint and Meteora TokenBadge, build the current IDART DBC configuration path, and successfully simulate a fresh DBC pool transaction against real AAPLx-compatible Mainnet state.

The broader xStocks registry remains compatibility-aware because individual assets can differ in Token-2022 extensions and mint configuration. IDART therefore inspects supported quote assets before exposing execution paths.

## PreStocks

IDART FUN currently exposes **8 PreStocks** in the Quote Asset Registry as part of the Stocklana product surface.

The PreStocks integration is being actively refined alongside the broader Token-2022 quote-asset compatibility work. The current public product keeps these assets visible in the registry while the team continues validating the most appropriate execution path for their specific mint configurations and welcomes ecosystem feedback as that work progresses.

---

# 🔎 Discovery Markets & Market Detail

The public product now includes a Discovery Markets layer:

https://idartfun.xyz/token/

The current interface exposes:

- market-status filtering
- quote-asset filtering
- search and sorting
- card / table views
- validated Mainnet and Devnet reference markets
- dedicated quote-market route visibility

The Mainnet MEMET validation market also has a dedicated public market-detail page:

https://idartfun.xyz/token/memet/

That page currently combines:

- project metadata
- launch configuration and economics
- Meteora DBC → DAMM v2 lifecycle information
- official GeckoTerminal market chart
- Jupiter embedded trading interface
- public fee / claim-status surfaces

The current MEMET page is the reference design for the future dynamic `/token/<mint>` market-detail system.

The next product step is automatic post-launch registration so a newly launched market can appear in Discovery and resolve into its own market-detail route without requiring a manually created WordPress page.

---

# 🧑‍💻 API for Builders — Coming Soon

IDART FUN is being designed so third-party builders can integrate its market infrastructure into dApps and websites without receiving IDART's proprietary application code.

## Planned integration options

- Low-code widgets / embeds
- Documented API
- SDK / transaction builders
- Custom partner integrations
- Market discovery endpoints
- Market-state endpoints
- Launch preparation
- Swap quote / transaction preparation
- Builder attribution

**Preview:**  
https://idartfun.xyz/idart-api-for-builders/

---

# 🔐 Security & Transaction Hardening

IDART FUN is non-custodial.

- Users sign their own transactions
- IDART never requests seed phrases or private keys
- Mainnet transactions are simulated before broadcast
- Broadcast transactions are not automatically resent when confirmation is uncertain
- Pending transactions are reconciled before retry
- Market recovery does not recreate an existing token or pool
- Risk acknowledgements are required before on-chain launch, swap, migration and claim actions

Following wallet-security feedback, the production transaction path is also being hardened around:

- Wallet-first signing order for multi-signer transactions
- Additional signers applied after wallet signing where required
- Transaction-size monitoring
- Address Lookup Tables where appropriate
- Preserving room for wallet security instructions
- Splitting oversized / excessive-compute workflows when necessary

---

# ⭐ What Makes IDART FUN Different

IDART FUN combines:

- Configurable market design
- Meteora DBC launch infrastructure
- Multiple quote-asset strategies
- Market Profiles
- Flexible fee economics
- Creator / holder / protocol incentive design
- Creator First Buy
- Graduation-safe PartialFill
- DAMM v2 graduation
- Multi-asset Quote Asset Registry with **1,274+ xStocks** and **8 PreStocks**
- Discovery Markets and dedicated market-detail experiences
- Planned Builder API, SDK and embeds

The goal is not merely to launch a token.

It is to let creators and builders define **how a market launches, what asset universe it trades against, how it graduates and how its economics are structured**.

For Creators, this expands possible market design and fee-generation paths beyond a single SOL or USDC pair.

For Holders, it expands the range of market exposure, quote-asset choice and future reward-oriented market economics available within the same launch infrastructure.

---

# 🏆 Stocklana 2026

IDART FUN was submitted to **Stocklana 2026** with a focus on:

- **Main Track**
- **Meteora — Best Use of DBC**
- **PreStocks — Best Use of PreStocks**

The project has continued evolving after submission.

Post-submission work is documented transparently and is **not retroactively presented as part of the original deadline build**.

Current post-submission progress now also includes:

- public Discovery Markets
- dedicated Mainnet market-detail experience
- **1,274+ xStocks** in the Quote Asset Registry
- **8 PreStocks** integrated into the quote catalog
- AAPLx-based Mainnet xStock compatibility validation through zero-cost RPC simulation

---

# 📚 Documentation

- [Architecture Overview](./ARCHITECTURE.md)
- [Market Design](./MARKET_DESIGN.md)
- [Economics](./ECONOMICS.md)
- [Submission Snapshot](./SUBMISSION_SNAPSHOT.md)
- [Roadmap](./ROADMAP.md)
- [Security](./SECURITY.md)
- [Mainnet Validation](./MAINNET_VALIDATION.md)

Implementation details, proprietary application code, deployment secrets, fee-routing implementation and internal market-configuration algorithms are intentionally not published in this showcase repository.

---

# 🏗️ Project Identity

IDART FUN began inside the broader IDART ecosystem and is now being developed as an independent launchpad and programmable market-infrastructure product.

The existing **IDARTDEX** GitHub account remains the owner of this Stocklana submission repository so the original hackathon URL and provenance remain stable during judging.

Future IDART FUN development can move to a dedicated IDART FUN GitHub presence without modifying this historical Stocklana submission record.

---

### IDART FUN

**Design the Market. Launch the Asset.**

© 2026 IDART FUN / IDART ecosystem.
