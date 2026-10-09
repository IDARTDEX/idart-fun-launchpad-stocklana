# Security

This repository is a public product showcase and contains no production secrets.

Never publish:

- seed phrases
- private keys
- wallet keypair files
- `.env` files
- RPC/API secrets
- authentication tokens
- deployment secrets

Security-sensitive implementation details are maintained outside this public showcase repository.

---

# 🔐 Non-Custodial Security Model

IDART FUN is non-custodial.

Users approve their own transactions and IDART FUN never requests a seed phrase, private key or wallet recovery phrase.

The product is designed around the principle:

## User Signs. IDART Never Holds the Key.

---

# Core Transaction Security Rules

The current product security model includes:

- transaction simulation before wallet approval when supported by the transaction path;
- no automatic resend solely because RPC confirmation is delayed;
- reconciliation of already-broadcast signatures before retry;
- recent blockhash and `lastValidBlockHeight` handling;
- preservation of valid Meteora ComputeBudget instructions;
- protection against duplicate token / config / pool creation during uncertain RPC reads;
- safety and risk acknowledgements before launch, swap, migration and claim-related actions;
- explicit separation between zero-cost diagnostic simulation and real Mainnet broadcast paths.

---

# 👛 Wallet-First Multi-Signer Handling

The hardened Mainnet signing path uses a wallet-first sequence for multi-signer transactions.

```js
// Wallet signs first
let signedTx = await signer.signTransaction(tx);

// Additional required signers are applied afterward
signedTx.partialSign(additionalSigner);
```

For flows that require temporary or position-related keypairs, the production path is designed to:

1. build the transaction;
2. simulate when appropriate;
3. request the wallet signature;
4. apply required additional signers afterward;
5. serialize and broadcast;
6. confirm using blockhash-aware expiry handling.

---

# 📦 Transaction Size Hardening

The current browser flow includes serialized transaction-size monitoring.

Production hardening includes:

- monitoring serialized transaction size;
- keeping transaction-size headroom for wallet security instructions;
- detecting oversized transactions before broadcast;
- avoiding unnecessary duplicate instructions;
- splitting oversized workflows when necessary;
- evaluating Address Lookup Tables where appropriate.

---

# ⚙️ Compute Budget Handling

The migration path preserves Meteora SDK ComputeBudget instructions when they are already present.

IDART FUN avoids injecting duplicate ComputeBudget instruction types into the same transaction.

This protects the DAMM v2 migration flow from duplicate-instruction failures.

---

# 🔁 Confirmation & Retry Safety

If a transaction is broadcast but confirmation is uncertain:

- store the submitted signature;
- check whether it landed before building a replacement transaction;
- do not assume a timeout means failure;
- treat blockhash expiry as distinct from RPC confirmation delay;
- only allow a retry after reconciliation.

This reduces the risk of duplicated user actions or duplicated on-chain operations.

---

# 🧪 Zero-Cost Mainnet Diagnostics

IDART FUN also uses Mainnet RPC simulation for compatibility testing where a real broadcast is not required.

The xStock compatibility diagnostic used for AAPLx:

- resolves real Mainnet state;
- builds the IDART DBC configuration path;
- builds a fresh pool transaction against AAPLx-compatible Mainnet state;
- runs `simulateTransaction`;
- requests no wallet signature;
- broadcasts nothing;
- spends `0 SOL`.

This allows protocol compatibility to be checked against real Mainnet state before deciding whether a paid transaction is necessary.

---

# 🛡️ Public Product Safety

The Launch interface includes safety and risk acknowledgements before on-chain transaction actions.

The public product also distinguishes:

- validated Mainnet / Devnet proof;
- public Discovery and market-detail experiences;
- compatibility diagnostics;
- future protocol modules such as the Holder Rewards Router.

This keeps product status visible without exposing private security implementation.

---

# Security Scope

These security and transaction-hardening improvements were completed as continued product development after the original Stocklana submission.

The original submission snapshot remains preserved separately in:

[`SUBMISSION_SNAPSHOT.md`](./SUBMISSION_SNAPSHOT.md)

---

# IDART FUN Security Principle

## User Signs. IDART Never Holds the Key.
