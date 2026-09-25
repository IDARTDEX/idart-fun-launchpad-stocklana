# Stocklana Submission Snapshot

**Hackathon deadline:** September 25, 2026

This file records the public product state at the Stocklana submission deadline.

## Available in the public launchpad interface

- responsive IDART launchpad UI
- Solana wallet connection
- token-launch configuration flow
- token metadata fields and image preview
- SOL / USDC / custom quote selection
- xStocks quote-market options
- PreStocks quote-market options
- Market Profile selection
- Economics Mode selection
- Meteora DBC configuration preparation
- exportable launch JSON
- IDART partner / fee-recipient setup
- visible Devnet engine proof

## End-to-end Devnet validation completed before the deadline

The Meteora DBC engine was validated separately from the browser UI with:

- DBC config creation
- token and virtual-pool creation
- real swaps
- creator and partner fee accrual
- `PartialFill` final buy that safely reached the migration threshold
- `100.00%` graduation
- successful DAMM v2 migration
- final `Migrated: yes` status confirmation

## In active integration at submission time

- direct web-interface broadcast of Meteora DBC launch transactions
- dynamic Explore registry
- individual Market pages
- integrated browser DBC Buy / Sell
- historical charts
- automated holder rewards

## Why this snapshot exists

IDART is an actively developed product and the live site will continue to change after Stocklana. This snapshot distinguishes the state submitted to the hackathon from later product improvements.
