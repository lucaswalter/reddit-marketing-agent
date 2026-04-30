---
title: Missing Cost Basis (MCB) — CoinLedger product concept
type: concept
jurisdiction: [global]
created: 2026-04-20
updated: 2026-04-20
tags: [coinledger-product, cost-basis, reconciliation, data-quality]
sources: [[coinledger-help-11648724-common-causes-of-missing-cost-basis-warnings-2026-04-20]], [[coinledger-help-2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-can-i-fix-it-2026-04-20]], [[coinledger-help-2599667-rounding-errors-missing-cost-basis-warning-2026-04-20]], [[coinledger-help-6811823-how-to-fix-first-inflow-missing-basis-warnings-2026-04-20]], [[coinledger-help-6105647-how-to-classify-nft-mint-transactions-and-remove-missing-cost-basis-warnings-2026-04-20]], [[coinledger-help-13264571-fixing-missing-cost-basis-issues-after-transitioning-to-per-wallet-cost-basis-tracking-2026-04-20]], [[coinledger-help-12609869-can-i-ignore-a-missing-cost-basis-warning-2026-04-20]], [[coinledger-help-2865416-can-i-file-my-taxes-with-an-unresolved-missing-cost-basis-2026-04-20]], [[coinledger-help-10080173-can-i-manually-enter-an-asset-s-cost-basis-aka-a-manual-position-2026-04-20]], [[coinledger-help-4357024-how-can-i-solve-a-historical-price-warning-2026-04-20]], [[coinledger-syntheses-coinledger-help-inventory-2026-04-20]]
---

## Definition

A **Missing Cost Basis (MCB)** warning is a CoinLedger-product-internal flag indicating that the system is unable to determine the cost basis of a disposed asset because the corresponding acquisition transaction is absent, malformed, or unreconciled [[coinledger-help-2552647-why-am-i-getting-a-missing-cost-basis-warning-and-how-can-i-fix-it-2026-04-20]]. If unresolved, the disposal will be reported with **$0 cost basis** — maximum taxable proceeds [[coinledger-help-12609869-can-i-ignore-a-missing-cost-basis-warning-2026-04-20]].

MCB is the single heaviest support theme in the CoinLedger help center — **at least nine dedicated articles** address sub-types and fix patterns [per the help-center inventory synthesis]. It is the canonical expression of real-world crypto-ledger imperfection and the primary user-facing UX surface for reconciliation work.

## The 11-cause taxonomy

Per [[coinledger-help-11648724-common-causes-of-missing-cost-basis-warnings-2026-04-20]] (the canonical root-cause explainer), MCB originates from discrete pipeline gaps:

1. **Missing exchange data** — API scope limits or user omission of a platform altogether.
2. **Missing years of history** — user imported 2023–2024 but not 2020–2022 where basis was established.
3. **Duplicate transactions** — the same buy imported twice, breaking lot sequencing.
4. **Uncategorized on-chain interactions** — contract calls CoinLedger couldn't classify, leaving inflow unassigned (see [[potential-bridges-trades-transfers]]).
5. **Coinbase ↔ Coinbase Pro split** — the legacy Pro account and main account had disjoint histories; pre-migration users who used both see basis gaps at the Pro side.
6. **MoonPay / Banxa / Transak on-ramps** — third-party fiat on-ramps that push crypto directly to a wallet with no acquisition record in the destination platform's API.
7. **Binance.US one-sided buys** — historical Binance.US API quirk where a buy appears as a deposit (no corresponding fiat-debit leg).
8. **Bridge merges** — cross-chain bridges that mint a wrapped or equivalent token on the destination chain without carrying basis metadata.
9. **Post-reallocation first-inflow** — following the Rev. Proc. 2024-28 reallocation (see [[per-wallet-cost-basis]]), a wallet's earliest-visible inflow may lack explicit basis from a prior Universal-view lot [[coinledger-help-6811823-how-to-fix-first-inflow-missing-basis-warnings-2026-04-20]], [[coinledger-help-13264571-fixing-missing-cost-basis-issues-after-transitioning-to-per-wallet-cost-basis-tracking-2026-04-20]].
10. **Rounding dust** — sub-satoshi quantities where calculated balance diverges from reported balance by rounding [[coinledger-help-2599667-rounding-errors-missing-cost-basis-warning-2026-04-20]].
11. **Self-custody wallet buys** — user bought crypto via an in-wallet swap (e.g., MetaMask Swaps) without connecting the swap-provider's data separately.

## Fix patterns

- **Connect the missing integration** — add the source exchange/wallet/on-ramp (most #1, #6, #7, #11).
- **Import historical CSVs** for years pre-dating API history (most #2, #5).
- **Remove duplicates** via the UI dedup tool (#3).
- **Classify via the PBT tab** — surface ambiguous on-chain transactions for user review (#4, #8) (see [[potential-bridges-trades-transfers]]).
- **Manually enter a Manual Position** — create a synthetic acquisition with user-specified basis and date [[coinledger-help-10080173-can-i-manually-enter-an-asset-s-cost-basis-aka-a-manual-position-2026-04-20]]. Works for any gap; requires user to know the basis.
- **Re-run reallocation** — for post-migration first-inflow cases [[coinledger-help-13264571-fixing-missing-cost-basis-issues-after-transitioning-to-per-wallet-cost-basis-tracking-2026-04-20]].
- **Accept $0 basis** — the user chooses to ignore the warning and file with maximum-proceeds treatment [[coinledger-help-12609869-can-i-ignore-a-missing-cost-basis-warning-2026-04-20]], [[coinledger-help-2865416-can-i-file-my-taxes-with-an-unresolved-missing-cost-basis-2026-04-20]]. Conservative; overpays tax; sometimes the right call when the true basis is unrecoverable.

## NFT-mint MCB

A specific sub-case: minting an NFT generates an inflow of a new-asset NFT with no corresponding "purchase" transaction. CoinLedger treats this via an explicit classification flow [[coinledger-help-6105647-how-to-classify-nft-mint-transactions-and-remove-missing-cost-basis-warnings-2026-04-20]] — the user confirms whether the mint cost (gas + mint fee) should be treated as the NFT basis.

## Related warnings

- **Historical Price Warning** [[coinledger-help-4357024-how-can-i-solve-a-historical-price-warning-2026-04-20]] — distinct from MCB but shares the reconciliation UX surface. Fires when CoinLedger cannot price a transaction at its historical moment (obscure token, thin-liquidity trade, timestamp before the token was priced). Resolution: user enters manual price, or removes/classifies the unreached transaction.

## Why it matters

- **Downstream tax impact.** Unresolved MCB → $0 basis → overreported gain → overpayment. For a user with 10 BTC at an unreconciled MoonPay on-ramp, the overpayment can be five figures.
- **Support-load concentration.** MCB is the single biggest support driver per the help-center inventory — CoinLedger has invested more documentation/article real estate here than on any other product surface.
- **Per-wallet migration amplification.** Rev. Proc. 2024-28 per-wallet tracking surfaced MCB warnings that were masked under Universal — the wallet's first visible inflow is now a hard basis question rather than an implicit draw from the shared pool.

## Related wiki pages

- [[per-wallet-cost-basis]], [[potential-bridges-trades-transfers]], [[universal-import-template]], [[form-8949]], [[cost-basis-methods]], [[spec-id]], [[coinledger]].

## Gaps

- Per-integration MCB rates — which exchanges / on-ramps generate the most warnings per user.
- Average time-to-resolution for each MCB cause.
- Whether MCB warnings can be issued at the wallet level in multi-user team accounts.
