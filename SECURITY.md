# Security

This repository is a public product showcase and contains no production secrets.

Do not publish:
- seed phrases
- private keys
- wallet keypair files
- `.env` files
- RPC/API secrets
- authentication tokens

Security-sensitive implementation details are maintained outside this public showcase repository.

# SECURITY UPDATE — OCTOBER 2026

> Add this section to the existing `SECURITY.md`.
>
> Keep the current Security content and append this block below it.

---

# 🔐 Wallet Security & Transaction Hardening

IDART FUN is non-custodial.

Users approve their own transactions and IDART FUN never requests a seed phrase, private key or wallet recovery phrase.

---

## Core Transaction Security Rules

- Simulate transactions before wallet approval when supported by the transaction path
- Never automatically resend a transaction only because RPC confirmation is delayed
- Reconcile an already-broadcast signature before allowing a retry
- Use recent blockhash and `lastValidBlockHeight` to identify expired or dropped transactions
- Preserve valid Meteora ComputeBudget instructions instead of injecting duplicate instruction types
- Never recreate a token, DBC config or pool merely because a read RPC failed
- Require safety and risk acknowledgements before launch, swap, migration and claim actions

---

# 👛 Phantom Compatibility

Following direct feedback from Phantom support, IDART FUN is updating multi-signer transaction handling to follow a **wallet-first signing sequence**.

## Recommended Signing Order

```js
// Phantom wallet signs first
let signedTx = await signer.signTransaction(tx);

// Additional signers sign afterward
signedTx.partialSign(additionalSigner);
```

For Meteora flows that return temporary or position-related keypairs, the production path should:

1. Build the transaction
2. Simulate when appropriate
3. Request the wallet signature first
4. Apply required additional signers afterward
5. Serialize and broadcast
6. Confirm using blockhash-aware expiry handling

---

# 📦 Transaction Size Hardening

Phantom support also identified that one of the validated transactions was approaching Solana's transaction-size limit.

Production hardening therefore includes:

- Monitoring serialized transaction size
- Using **Address Lookup Tables (ALT)** where appropriate
- Leaving room for wallet security / Lighthouse instructions
- Avoiding unnecessary duplicate instructions
- Splitting oversized or excessive-compute workflows when necessary

---

# ⚙️ Compute Budget Handling

The migration path must preserve Meteora SDK ComputeBudget instructions when they are already present.

IDART FUN should not inject duplicate ComputeBudget instruction types into the same transaction.

This avoids failures such as duplicate instruction errors during DAMM v2 migration.

---

# 🔁 Confirmation & Retry Safety

If a transaction is broadcast but confirmation is uncertain:

- Store the submitted signature
- Check whether it landed before building a replacement transaction
- Do not assume a timeout means failure
- Treat blockhash expiry as distinct from RPC confirmation delay
- Only allow a retry after reconciliation

This reduces the risk of duplicated user actions or duplicated on-chain operations.

---

# 🧾 Security Scope

These changes are **production-hardening improvements completed after the original Stocklana submission**.

They should not be presented as features that existed at the original hackathon deadline.

---

# IDART FUN Security Principle

## User Signs. IDART Never Holds the Key.
