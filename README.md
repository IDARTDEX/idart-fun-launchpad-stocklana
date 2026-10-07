IDART FUN
Design the Market. Launch the Asset.
IDART FUN is a Solana-native programmable market launchpad built on Meteora Dynamic Bonding Curve (DBC).
Creators can configure how a market launches instead of using one fixed template: token, quote asset, Market Profile, economics mode, creator first buy, bonding path and graduation to Meteora DAMM v2.
Stocklana submission repository
This repository remains the public record of the IDART FUN Stocklana 2026 submission.
The original submission state is preserved in [`SUBMISSION_SNAPSHOT.md`](./SUBMISSION_SNAPSHOT.md).
The sections marked Post-Submission Progress document development completed after the submission deadline and are not presented as features that existed at submission time.
________________________________________
Live Product
•	IDART FUN: https://idartfun.xyz
•	Launch: https://idartfun.xyz/launch/
•	API for Builders — Coming Soon: https://idartfun.xyz/idart-api-for-builders/
•	X: https://x.com/IDARTFun_Launch
•	Legacy submission URL: https://launchpad.idartdex.xyz → redirects to the current IDART FUN domain
IDART FUN is now being developed as an independent product within the broader IDART ecosystem.
________________________________________
Post-Submission Progress · October 2026
Since the Stocklana submission, IDART FUN has progressed from its submitted MVP into a substantially more complete launchpad with a validated browser-native lifecycle.
Core lifecycle now validated
•	✅ Solana Devnet end-to-end launch
•	✅ Solana Mainnet end-to-end launch with real SOL
•	✅ Meteora DBC config + pool creation
•	✅ wallet-signed swaps
•	✅ creator first buy / Dev Buy
•	✅ live bonding progress
•	✅ graduation-safe PartialFill
•	✅ 100% bonding
•	✅ successful DBC → DAMM v2 migration
•	✅ creator and partner fee accrual
•	✅ recovery of an existing market without recreating the token or pool
•	✅ public Mainnet and Devnet validation archives in the Launch UI
Product layer now available
•	configurable Market Profiles
•	configurable Economics modes
•	production Mainnet market-cap targets
•	public token metadata preparation
•	project links / social metadata fields
•	Launch Review before transaction signing
•	mandatory safety and risk acknowledgements
•	browser wallet integration
•	Mainnet transaction simulation before approval
•	Discovery Markets foundation
•	API for Builders preview
•	responsive desktop/mobile UI
In active development
•	Holder Rewards Router and holder claims
•	real Discovery market indexing
•	Market Detail pages and analytics
•	xStocks / PreStocks Quote Asset Registry
•	Token-2022 compatibility filtering
•	Builders API / SDK / low-code embeds
•	partner attribution and builder-originated transaction economics
•	transaction-size hardening using Address Lookup Tables where appropriate
•	additional wallet-security compatibility improvements
________________________________________
Verified Mainnet Lifecycle
A real IDART FUN Mainnet market was launched and graduated through the full lifecycle:
Create → Meteora DBC → Buy / Trade → 100% Bonding → DAMM v2
Mainnet validation market
•	Token: Meme Tesla Club Test
•	Symbol: MEMET
•	Base Mint: 3qekQqW4YLLTjNPfaSB8AaQ9MUpTcthck4qKARM7uhSL
•	DBC Pool: 2K1PYMVUChhBLPwfQ5ZAjgFwVTPXa34UKdGJkQwrrTFm
•	Network: Solana Mainnet
•	Final Bonding: 100%
•	Final Migration: DAMM v2
•	Status: Migrated
Mainnet proof
•	Launch + initial buy transaction:
https://explorer.solana.com/tx/5SPwDnURxJeANhUJawmb9Zb7cifBZcMnCgTtwgCwSTJ9Xy2Sz4MeYGgTp61QscAjxKLqEhriiCgEspbgm3jMPU4R
•	Base Mint:
https://explorer.solana.com/address/3qekQqW4YLLTjNPfaSB8AaQ9MUpTcthck4qKARM7uhSL
•	DBC Pool:
https://explorer.solana.com/address/2K1PYMVUChhBLPwfQ5ZAjgFwVTPXa34UKdGJkQwrrTFm
•	Market view:
https://dexscreener.com/solana/2k1pymvuchhblpwfq5zajgfwvtpxa34ukdgjkqwrrtfm
The live Launch page also exposes a Verified Mainnet Validation Archive so evaluators can inspect the completed lifecycle without initiating another Mainnet test.
No additional Mainnet testing is required for the Stocklana evaluation. Future Mainnet validations will be performed only when necessary for new protocol features.
________________________________________
Verified Devnet Lifecycle
The original Devnet validation remains part of the submission evidence.
Devnet identifiers
•	Base Mint: 8B1cJpMukfEbK5wJYixSnkpn5eGZWPpmtrRVPbYtPXZz
•	DBC Pool: DYi5X52fshUZ3fYnex8Jbs1usFS5vT9zTAC4Tz4ooYEA
•	DBC Config: DpLXcMud36KpyC6dxZQrjHyJRetWeF3M3yf6TsR2T9sC
Devnet transactions
•	Create Config: 5bHRDBH6eU39M9fTo6XKoFJpXpLsk54WyzU3YP9XwctEkbVU23YjSZ3Nri6ZpihsgSFdP4NYgvqVjrmo113EBxMc
•	Create Pool: 5pnrQCLxri2qhrZkJAb8KUEnFymtLEK53S2qzZiPKYQqJGXwF4fuzrH3meCZR2gvq5MEfqmsatcroMYj4p2fVnJv
•	First Swap: 5ovFiywgwuXbsZcJ3uVGLDLnkkbtXVsfYSNpDp5JYqFE7SKadUCqEcTfQGGgHZuePqDGiSQjAPotCavKX4sKQeEr
•	Graduation-safe PartialFill: r8Vvmoi6g2CVJbsoEJJ76d7rNFefa4q751gr3ifLJyWuR2Toy4StftkvT4rqYrJZsbw2pyHDQ94MqTSHzUoqnvm
The Devnet validation demonstrated:
•	real config and pool creation
•	real swaps
•	creator / partner fee accrual
•	graduation-safe PartialFill
•	100% bonding
•	successful DAMM v2 migration
________________________________________
Market Design
IDART FUN is designed as a market-design layer over Meteora, not only a token generator.
Market Profiles
Profile	Starting MC Reference	Graduation MC Reference	Intent
Discovery	28 SOL	300 SOL	early price discovery
Balanced	35 SOL	350 SOL	general-purpose launches
Asset Quote	40 SOL	450 SOL	quote-asset / RWA-style markets
These are market-cap references used by the launch configuration, not claims about guaranteed liquidity or token value.
Economics Modes
The public design keeps the total trading fee fixed at 2.50% while changing the allocation logic.
Economics Mode	Creator	Holder Allocation	Protocol
Creator First · Standard	60%	10%	30%
All Win · Balanced	35%	35%	30%
Holder Rewards · Community	10%	60%	30%
Meteora DBC provides native creator / partner fee accounting.
IDART's holder-by-holder Rewards Router is a separate protocol layer and remains under active development; the public product does not claim that holder claims are fully deployed until that router is live.
________________________________________
Creator First Buy / Dev Buy
Creators may optionally participate in the launch transaction with a first buy.
The production UI supports a configurable creator first-buy percentage and recalculates the exact Meteora quote before signing.
As a reference, a 5% creator first buy under the Discovery starting market-cap profile is approximately 1.5 SOL, but the actual transaction quote is authoritative.
________________________________________
Quote Markets
IDART FUN is being designed to support:
•	SOL
•	USDC
•	compatible Solana SPL tokens
•	compatible Token-2022 assets
•	xStocks / tokenized public equities
•	compatible PreStocks / pre-IPO market assets
Meteora ecosystem guidance confirmed that Token-2022 xStocks can be used as DBC quote mints and that Scaled UI Amount is not itself a blocker. IDART is building its own Quote Asset Registry to inspect mint properties and expose only supported configurations.
Transfer Hook assets require additional DAMM v2 compatibility handling and are treated separately.
________________________________________
API for Builders · Coming Soon
IDART FUN is being designed so third-party builders can integrate the market layer into dApps and websites without receiving IDART's proprietary application code.
Planned integration levels include:
•	Low-code widgets / embeds
•	documented API
•	SDK / transaction builders
•	custom partner integrations
•	market discovery and market-state endpoints
•	launch preparation
•	swap quote / transaction preparation
•	builder attribution
Preview:
https://idartfun.xyz/idart-api-for-builders/
________________________________________
Security & Transaction Hardening
IDART FUN is non-custodial:
•	users sign their own transactions
•	IDART never requests seed phrases or private keys
•	Mainnet transactions are simulated before broadcast
•	broadcast transactions are not automatically resent when confirmation is uncertain
•	pending transactions are reconciled before retry
•	market recovery does not recreate an existing token or pool
•	risk acknowledgements are required before on-chain launch, swap, migration and claim actions
Following wallet-security feedback, the production transaction path is also being hardened around:
•	wallet-first signing order for multi-signer transactions
•	additional signers applied after wallet signing where required
•	transaction-size monitoring
•	Address Lookup Tables where appropriate
•	preserving room for wallet security instructions
•	splitting oversized / excessive-compute workflows when necessary
________________________________________
What Makes IDART FUN Different
IDART FUN combines:
•	configurable market design
•	Meteora DBC launch infrastructure
•	multiple quote-asset strategies
•	Market Profiles
•	flexible fee economics
•	creator / holder / protocol incentive design
•	creator first buy
•	graduation-safe PartialFill
•	DAMM v2 graduation
•	planned stock-token / PreStock quote markets
•	planned Builder API, SDK and embeds
The goal is not merely to launch a token. It is to let creators and builders define how a market launches, how it graduates and how its economics are structured.
________________________________________
Stocklana 2026
IDART FUN was submitted to Stocklana 2026 with a focus on:
•	Main Track
•	Meteora — Best Use of DBC
•	PreStocks — Best Use of PreStocks
The project has continued evolving after submission.
Post-submission work is documented transparently and is not retroactively presented as part of the original deadline build.
________________________________________
Documentation
•	[Architecture Overview](./ARCHITECTURE.md)
•	[Market Design](./MARKET_DESIGN.md)
•	[Economics](./ECONOMICS.md)
•	[Submission Snapshot](./SUBMISSION_SNAPSHOT.md)
•	[Roadmap](./ROADMAP.md)
•	[Security](./SECURITY.md)
•	[Mainnet Validation](./MAINNET_VALIDATION.md)
Implementation details, proprietary application code, deployment secrets, fee-routing implementation and internal market-configuration algorithms are intentionally not published in this showcase repository.
________________________________________
Project Identity
IDART FUN began inside the broader IDART ecosystem and is now being developed as an independent launchpad and programmable market-infrastructure product.
The existing IDARTDEX GitHub organization remains the owner of this Stocklana submission repository so the original hackathon URL and provenance stay stable throughout judging.
Future IDART FUN development may move to a dedicated IDART FUN organization/repository without modifying the historical Stocklana submission record.
________________________________________
© 2026 IDART FUN / IDART ecosystem.

