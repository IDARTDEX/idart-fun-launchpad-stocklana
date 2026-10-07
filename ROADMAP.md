# IDART FUN ROADMAP

## Programmable Market Infrastructure on Solana

**IDART FUN** is evolving from a configurable launchpad into a broader programmable market-infrastructure layer built on **Meteora Dynamic Bonding Curve (DBC)** and Solana.

This roadmap reflects the current project status after the original Stocklana submission and the subsequent Devnet and Mainnet validation work.

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

- [x] **Discovery**
  - Starting MC reference: `28 SOL`
  - Graduation MC reference: `300 SOL`

- [x] **Balanced**
  - Starting MC reference: `35 SOL`
  - Graduation MC reference: `350 SOL`

- [x] **Asset Quote**
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
- [x] Dedicated IDART FUN X profile
- [x] Legacy Stocklana URL redirected to the current domain
- [x] Responsive desktop and mobile interface
- [x] Dedicated Builders API preview page

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

# 🚧 Phase 4 — Discovery Markets

## Status: Next Priority

The next major product milestone is to turn IDART FUN from a launch interface into a navigable market-discovery platform.

### Planned

- [ ] Index real IDART launches
- [ ] Market cards
- [ ] Token / symbol search
- [ ] Filter by network
- [ ] Filter by quote asset
- [ ] Filter by Market Profile
- [ ] Filter by Economics mode
- [ ] Sort by market cap
- [ ] Sort by volume
- [ ] Sort by bonding progress
- [ ] Graduation status
- [ ] DAMM v2 migration status
- [ ] Recently launched markets
- [ ] Trending markets

### Data Sources

Planned architecture should prioritize:

- On-chain Meteora state
- Jupiter metadata
- GeckoTerminal
- Birdeye fallback
- Internal IDART indexing

Paid DexScreener metadata services are not required for the core product.

---

# 🚧 Phase 5 — Market Detail Pages

## Status: Planned

Each launched market should have a dedicated page.

### Planned Market Data

- [ ] Token name
- [ ] Symbol
- [ ] Logo
- [ ] Base Mint
- [ ] Quote Mint
- [ ] Market Profile
- [ ] Economics mode
- [ ] Starting MC
- [ ] Current MC
- [ ] Graduation MC
- [ ] Bonding progress
- [ ] Migration state
- [ ] Creator fee accrual
- [ ] Partner / protocol fee accrual
- [ ] Holder allocation accounting
- [ ] Volume
- [ ] Liquidity
- [ ] Holders
- [ ] Transaction history
- [ ] Project links
- [ ] Metadata
- [ ] Explorer links

### Trading Experience

- [ ] Buy / Sell interface
- [ ] Swap quote preview
- [ ] Slippage settings
- [ ] Transaction simulation
- [ ] Wallet confirmation
- [ ] Explorer transaction link

---

# 🚧 Phase 6 — Quote Asset Registry

## Status: Planned / Technical Validation Underway

IDART FUN is being designed to support programmable quote markets beyond SOL.

### Initial Quote Assets

- [x] SOL
- [ ] USDC
- [ ] Compatible SPL tokens
- [ ] Compatible Token-2022 tokens
- [ ] xStocks
- [ ] Compatible PreStocks

### xStocks / Token-2022 Direction

Meteora ecosystem guidance confirmed that Token-2022 xStocks can be used as `quoteMint` in DBC.

Scaled UI Amount is not itself considered a blocker.

Transfer Hook assets require separate DAMM v2 compatibility handling.

### Registry Validation

The IDART Quote Asset Registry should inspect:

- [ ] Mint address
- [ ] Token program
- [ ] Decimals
- [ ] Supply
- [ ] Metadata
- [ ] Token-2022 extensions
- [ ] Scaled UI Amount
- [ ] Transfer Hook
- [ ] Transfer Fee
- [ ] Permanent Delegate
- [ ] Mint Close Authority
- [ ] Freeze Authority
- [ ] Compatibility flags
- [ ] Allow / reject status

### Goal

Only quote assets validated as compatible should be exposed in the Launch UI.

---

# 🚧 Phase 7 — Holder Rewards Router

## Status: High Priority

Meteora DBC provides native Creator and Partner fee accounting.

IDART's economics model requires an additional protocol layer to distribute the holder allocation transparently.

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

### Important

The public product should not claim that holder-by-holder rewards are fully deployed until this router is live.

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

- [ ] Wallet-first multi-signer handling
- [ ] Additional signers after wallet signing where required
- [ ] Phantom Lighthouse compatibility improvements
- [ ] Multi-wallet compatibility testing

### Transaction Size

- [ ] Serialized transaction size monitoring
- [ ] Address Lookup Table support
- [ ] Room for wallet security instructions
- [ ] Oversized transaction splitting

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
- [ ] Smart-contract / protocol-layer review where applicable
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
- [ ] RWA-oriented profiles
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

The Stocklana submission repository should remain stable during judging.

Do not rename, transfer or rewrite its history before judging is complete.

## World's Fair

Planned preparation:

- [ ] Dedicated IDART FUN GitHub presence
- [ ] Updated product video
- [ ] Updated architecture documentation
- [ ] Discovery Markets
- [ ] Market Detail pages
- [ ] Quote Asset Registry
- [ ] Holder Rewards Router progress
- [ ] Builders API progress
- [ ] Security hardening
- [ ] Mainnet product evidence

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

---

# IDART FUN

## Design the Market. Launch the Asset.
