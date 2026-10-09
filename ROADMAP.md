# IDART FUN ROADMAP

## Programmable Market Infrastructure on Solana

**IDART FUN** is evolving from a configurable launchpad into a broader programmable market-infrastructure layer built on **Meteora Dynamic Bonding Curve (DBC)** and Solana.

This roadmap reflects the current project status after the original Stocklana submission and the subsequent Devnet, Mainnet, Discovery Markets, token-detail and multi-asset quote-market validation work.

---

# ✅ Phase 1 — Core Launch Infrastructure

## Status: Validated

The core launch lifecycle has been validated end-to-end.

### Completed

- [x] Solana wallet connection
- [x] Browser-native launch flow
- [x] Meteora DBC config creation
- [x] Token / virtual pool creation
- [x] Creator First Buy / Dev Buy
- [x] Wallet-signed swaps
- [x] Live bonding progress
- [x] Graduation-safe `PartialFill`
- [x] 100% bonding
- [x] DBC → DAMM v2 migration
- [x] Creator / partner fee accrual
- [x] Existing-market recovery
- [x] Mainnet transaction simulation
- [x] Devnet end-to-end validation
- [x] Mainnet end-to-end validation with real SOL
- [x] Devnet validation archive
- [x] Mainnet validation archive

---

# ✅ Phase 2 — Production Market Design

## Status: Implemented / Active

IDART FUN introduces configurable market design instead of a single fixed launch configuration.

### Market Profiles

- [x] **⚡ Lightning**
  - Starting MC reference: `28 SOL`
  - Graduation MC reference: `300 SOL`

- [x] **⚖️ Smooth Graduation**
  - Starting MC reference: `35 SOL`
  - Graduation MC reference: `350 SOL`

- [x] **📈 Scale Up**
  - Starting MC reference: `40 SOL`
  - Graduation MC reference: `450 SOL`

### Economics Modes

- [x] **Creator First · Standard**
  - Creator: `60%`
  - Holder Allocation: `10%`
  - Protocol: `30%`

- [x] **All Win · Balanced**
  - Creator: `35%`
  - Holder Allocation: `35%`
  - Protocol: `30%`

- [x] **Holder Rewards · Community**
  - Creator: `10%`
  - Holder Allocation: `60%`
  - Protocol: `30%`

### Trading Fee

- [x] Fixed total trading fee: `2.50%`

### LP Protection Design

- [x] `80%` Permanent Locked LP
- [x] `20%` Protocol Reserve LP
- [x] `90-day` vesting for Protocol Reserve LP
- [x] `0%` Creator Withdrawable LP

---

# ✅ Phase 3 — Product Identity & Public Launch Layer

## Status: Implemented

### Product Identity

- [x] Dedicated domain: `https://idartfun.xyz`
- [x] Dedicated Launch page
- [x] Dedicated Discovery Markets page
- [x] Dedicated token-market index at `/token/`
- [x] Dedicated Mainnet market-detail page for MEMET
- [x] Dedicated IDART FUN X profile
- [x] Legacy Stocklana URL redirected to the current domain
- [x] Responsive desktop, tablet and mobile interface
- [x] Dedicated Builders API preview page
- [x] Public GitHub links surfaced in the product UI
- [x] Dedicated Privacy Policy page

### Public Launch UX

- [x] Token metadata fields
- [x] Website and social fields
- [x] Launch Review
- [x] Safety and risk acknowledgements
- [x] Mainnet / Devnet status visibility
- [x] Bonding progress
- [x] Migration state
- [x] Fee visibility
- [x] Validation archive

---

# ✅ Phase 4 — Discovery Markets

## Status: Public Product Layer Live

Discovery Markets is now a public navigable surface rather than a future-only milestone.

### Implemented

- [x] Public market cards
- [x] Token / symbol search
- [x] Quote-asset filtering
- [x] Market-status filtering
- [x] Sorting controls
- [x] Card / table views
- [x] Mainnet MEMET reference market
- [x] Devnet IDDEMO reference market
- [x] xStocks route visibility
- [x] PreStocks route visibility
- [x] USDC route visibility
- [x] Solana-token quote route visibility
- [x] Graduation / migration state visibility

### Data Sources

The product layer prioritizes:

- On-chain Meteora state
- Jupiter metadata
- GeckoTerminal
- Public token registries
- Internal IDART market indexing

### Next Step

- [ ] Automatically register new IDART-originated launches in Discovery immediately after confirmed market creation
- [ ] Populate indexed market-cap, volume, liquidity and holder fields from live data sources

---

# ✅ Phase 5 — Market Detail Pages

## Status: Mainnet Reference Page Live / Dynamic Routing Next

The Mainnet MEMET market-detail page now serves as the reference design for future dynamically generated token pages.

### Implemented on the MEMET reference page

- [x] Token name
- [x] Symbol
- [x] Logo
- [x] Base Mint
- [x] DBC Pool
- [x] Market Profile
- [x] Economics mode
- [x] Launch configuration
- [x] Migration state
- [x] Project links
- [x] Public metadata
- [x] Explorer links
- [x] Official GeckoTerminal chart integration
- [x] Jupiter embedded trading interface
- [x] Fee / claim-status surfaces

### Next Step

- [ ] Dynamic `/token/<mint>` routing
- [ ] Automatic page hydration from registry + on-chain + metadata sources
- [ ] Live indexed market cap
- [ ] Live liquidity
- [ ] Live volume
- [ ] Holder count
- [ ] Transaction history
- [ ] Wallet-aware claim surfaces when the Holder Rewards Router is live

---

# ✅ Phase 6 — Quote Asset Registry

## Status: Public Registry Live / Multi-Asset Validation Active

IDART FUN is designed to support programmable quote markets beyond SOL.

### Current Quote Surfaces

- [x] SOL
- [x] USDC surfaced in the product
- [x] Compatible Solana SPL-token route surfaced
- [x] Compatible Token-2022 inspection
- [x] **1,274+ xStocks** discoverable through the current Quote Asset Registry
- [x] **8 PreStocks** integrated into the current quote catalog

### xStocks Mainnet Compatibility

The xStock quote-market path has been validated against real Solana Mainnet state using **AAPLx** as the representative stock-quote asset.

- [x] Real AAPLx quote mint resolved
- [x] Token-2022 inspection
- [x] Meteora TokenBadge resolved
- [x] IDART exact DBC config simulation: PASS
- [x] Fresh AAPLx `createPool` builder: PASS
- [x] Fresh AAPLx Mainnet simulation: PASS
- [x] Zero-cost validation path: `0 SOL`
- [x] No wallet signature or broadcast required for the compatibility test

### Registry Inspection

The registry architecture inspects:

- [x] Mint address
- [x] Token program
- [x] Decimals
- [x] Metadata
- [x] Token-2022 extensions
- [x] Scaled UI Amount
- [x] Transfer Hook
- [x] Transfer Fee configuration
- [x] TokenBadge availability where applicable
- [x] Compatibility state

### PreStocks

Eight PreStocks are integrated into the public quote catalog as part of the Stocklana product surface.

The team is continuing compatibility validation across their specific Token-2022 mint configurations while keeping the registry integration and product UX available for evaluation.

---

# 🚧 Phase 7 — Holder Rewards Router

## Status: High Priority

Meteora DBC provides native Creator and Partner fee accounting.

IDART's economics model adds a protocol layer intended to make holder allocations transparent and claimable.

### Planned

- [ ] Holder allocation accounting
- [ ] Reward entitlement model
- [ ] Snapshot / eligibility logic
- [ ] Claimable balance
- [ ] Holder claim transaction
- [ ] Claim history
- [ ] Protocol-side accounting
- [ ] Transparent reward reporting
- [ ] Security review

---

# 🚧 Phase 8 — API for Builders

## Status: Preview Live / Product Development Planned

IDART FUN is being designed as infrastructure that third-party builders can integrate without receiving IDART's proprietary application code.

### Planned API Capabilities

- [ ] `GET /v1/markets`
- [ ] `GET /v1/markets/:mint`
- [ ] `POST /v1/launch/prepare`
- [ ] `POST /v1/swap/quote`
- [ ] `POST /v1/swap/build`

### Planned SDK Capabilities

- [ ] Launch preparation
- [ ] Market state
- [ ] Swap quote generation
- [ ] Transaction builders
- [ ] Migration state
- [ ] Fee state
- [ ] Quote Asset Registry access

### Planned Embeds

- [ ] Launch Widget
- [ ] Market Widget
- [ ] Trade Widget
- [ ] Discovery Widget

### Builder Economics

- [ ] Builder attribution
- [ ] Partner-originated transaction tracking
- [ ] Protocol-side fee attribution
- [ ] Builder incentives

### Preview

https://idartfun.xyz/idart-api-for-builders/

---

# 🔐 Phase 9 — Security & Transaction Hardening

## Status: Active

### Wallet Compatibility

- [x] Wallet-first signing order for the current hardened Mainnet path
- [x] Additional signers applied after wallet signing where required
- [x] Transaction-size guards in the current browser flow
- [ ] Expanded multi-wallet compatibility testing
- [ ] Additional wallet-security compatibility improvements

### Transaction Size

- [x] Serialized transaction size monitoring
- [ ] Address Lookup Table support where appropriate
- [x] Room preserved for wallet-security instructions
- [x] Oversized-transaction detection

### Confirmation & Retry Safety

- [x] Blockhash-aware expiry handling
- [x] Broadcast signature storage
- [x] Pending transaction reconciliation
- [x] Safe retry logic
- [x] Existing-market recovery
- [x] ComputeBudget deduplication

### Infrastructure

- [ ] Dedicated production RPC
- [ ] Redundant RPC fallback
- [ ] Reliable indexing
- [ ] Monitoring
- [ ] Logging
- [ ] Alerting

### Security Review

- [ ] External code review
- [ ] Protocol-layer review where applicable
- [ ] API security review
- [ ] Holder Rewards Router review
- [ ] Production launch checklist

---

# 🔭 Phase 10 — Advanced Market Infrastructure

## Status: Future

### Advanced Economics

- [ ] Curator / KOL fee sharing
- [ ] Community Boost
- [ ] Referral economics
- [ ] Builder incentives
- [ ] Partner economics

### Advanced Market Design

- [ ] Additional Market Profiles
- [ ] Custom liquidity shapes
- [ ] Custom graduation templates
- [ ] Additional RWA-oriented profiles
- [ ] Stock-quote market templates
- [ ] PreStock market templates

### Liquidity Infrastructure

- [ ] DAMM v2 enhancements
- [ ] DLMM Pro evaluation
- [ ] Advanced post-graduation liquidity options

---

# 🌐 Phase 11 — IDART Ecosystem Expansion

## Status: Long-Term

IDART FUN is being developed as an independent product within the broader IDART ecosystem.

### Ecosystem Direction

- IDART FUN — programmable market launch infrastructure
- IDART DEX — trading and exchange products
- Future IDART Web3 products

Each product should maintain its own identity, roadmap and user base while remaining capable of supporting the broader ecosystem.

---

# 🏆 Hackathon & Ecosystem Strategy

## Stocklana 2026

- [x] Submission completed
- [x] Public repository
- [x] Devnet proof
- [x] Post-submission browser validation
- [x] Mainnet end-to-end validation
- [x] Verified DAMM v2 migration proof
- [x] Discovery Markets public layer
- [x] Mainnet market-detail reference page
- [x] 1,274+ xStocks registry
- [x] 8 PreStocks integrated into the quote catalog
- [x] AAPLx xStock Mainnet compatibility simulation

The Stocklana submission repository should remain stable during judging.

Do not rename, transfer or rewrite its history before judging is complete.

## World's Fair

Preparation focus:

- [ ] Dedicated IDART FUN GitHub presence after Stocklana judging
- [ ] Updated product video
- [x] Updated architecture documentation
- [x] Discovery Markets
- [x] Mainnet market-detail reference page
- [x] Quote Asset Registry
- [ ] Automatic post-launch Discovery registration
- [ ] Dynamic `/token/<mint>` market pages
- [ ] Holder Rewards Router progress
- [ ] Builders API progress
- [ ] Additional security hardening
- [x] Mainnet product evidence

---

# 🎯 Product Vision

IDART FUN is not intended to be only a token launcher.

The long-term goal is to become a **programmable market-design layer for Solana**, where creators, protocols and builders can define:

- how a market launches;
- what quote asset it uses;
- how the bonding curve behaves;
- how fees are allocated;
- how holders participate;
- how the market graduates;
- and how the infrastructure can be embedded into third-party products.

The product direction is to connect token creation, configurable economics, multi-asset quote markets, Discovery and market-detail experiences into one coherent launch-to-market lifecycle.

---

# IDART FUN

## Design the Market. Launch the Asset.
