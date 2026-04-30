---
title: Potential Bridges, Trades and Transfers (PBT) — CoinLedger product concept
type: concept
jurisdiction: [global]
created: 2026-04-20
updated: 2026-04-20
tags: [coinledger-product, reconciliation, on-chain, classification]
sources: [[coinledger-help-10714995-what-is-the-potential-bridges-trades-and-transfers-tab-2026-04-20]], [[coinledger-syntheses-coinledger-help-inventory-2026-04-20]]
---

## Definition

The **Potential Bridges, Trades and Transfers** tab (internally and in support articles abbreviated "PBT") is a CoinLedger UI surface where the product exposes **ambiguous on-chain transactions** for user review and manual classification [[coinledger-help-10714995-what-is-the-potential-bridges-trades-and-transfers-tab-2026-04-20]]. The tab is one of the two main reconciliation surfaces in the product (the other being the [[missing-cost-basis]] warning queue).

Per the help-center synthesis, PBT is flagged as one of the "standouts for product insight" — it reveals how CoinLedger heuristically models bridge, trade, and transfer detection across on-chain activity [per [[coinledger-syntheses-coinledger-help-inventory-2026-04-20]]].

## What gets flagged and why

On-chain activity is fundamentally harder to classify than exchange activity. Exchanges send labeled data (buy, sell, deposit, withdraw); blockchains emit transfers and contract calls without built-in accounting semantics. CoinLedger's ingestion engine attempts automatic classification and surfaces **cases it can't classify confidently** to the PBT tab [[coinledger-help-10714995-what-is-the-potential-bridges-trades-and-transfers-tab-2026-04-20]]:

- **Unreconciled pairs** — an outflow from one address/chain that doesn't have a clean matching inflow at another known address within the expected time window. Could be a bridge, an unsupported DEX swap, or a transfer to an unknown wallet.
- **Cross-chain bridge candidates** — an outflow on chain A followed by an inflow on chain B of a wrapped or equivalent asset, with the match ambiguous enough that CoinLedger asks the user to confirm (disposal vs. non-taxable transfer).
- **DEX swap candidates** — contract interactions that look like swaps but where the protocol isn't in CoinLedger's classifier database.
- **Ambiguous transfer vs. trade** — an on-chain movement that could be internal (same user, non-taxable) or external (third-party disposal).

## User disposition options

From the PBT tab, the user classifies each entry to one of a small set of outcomes [[coinledger-help-10714995-what-is-the-potential-bridges-trades-and-transfers-tab-2026-04-20]]:

- **Trade** — treats as a crypto-to-crypto disposal. Triggers basis lookup on the disposed asset and sets the received asset's basis to proceeds.
- **Bridge** — treats as a non-taxable transfer; basis carries across chains. Critical for wrapped-token flows (e.g., ETH → stETH treated as bridge in some jurisdictions).
- **Transfer** — wallet-to-wallet within the same user; non-taxable; basis preserved.
- **Ignore / mark as classified** — user suppresses the flag.

Each classification has downstream tax-character consequences. Misclassifying a trade as a transfer suppresses a taxable event; misclassifying a transfer as a trade creates a spurious gain.

## Why it matters

- **On-chain activity is the dominant reconciliation surface** for DeFi-active users. The PBT queue is where the bulk of DeFi, multi-chain, and bridge-heavy users resolve their year [[coinledger-syntheses-coinledger-help-inventory-2026-04-20]].
- **UK DeFi classification depends on it.** HMRC's CRYPTO61674 guidance distinguishes collateral deposit (non-disposal if beneficial ownership retained) from LP token (disposal). PBT is where the user encodes that distinction (see [[defi-tax-treatment]]).
- **Bridge treatment is jurisdictionally unresolved.** No ingested source gives a bright-line "bridge is not a disposal" rule for any jurisdiction. CoinLedger defers to user classification; the user effectively takes the position.
- **Load-bearing for MCB prevention.** A misclassified on-chain event can cascade into [[missing-cost-basis]] warnings downstream — the "uncategorized on-chain interactions" line item in the MCB taxonomy is the PBT tab's untaken action [[coinledger-help-11648724-common-causes-of-missing-cost-basis-warnings-2026-04-20]].

## Relationship to other reconciliation surfaces

- **Missing Cost Basis (MCB)** warnings fire when a disposal can't find a basis (see [[missing-cost-basis]]).
- **Historical Price Warning** fires when a transaction can't be priced at its moment [[coinledger-help-4357024-how-can-i-solve-a-historical-price-warning-2026-04-20]].
- **PBT** fires before either — it's the "what kind of transaction is this" layer.

In a clean reconciliation flow: PBT classification → MCB gap detection → Historical Price Warning resolution → [[form-8949]] generation.

## Related wiki pages

- [[missing-cost-basis]], [[defi-tax-treatment]], [[universal-import-template]], [[form-8949]], [[coinledger]].

## Primary guidance

- No regulator guidance directly addresses bridge/swap classification heuristics — this is a product-level construct.

## Gaps

- Per-protocol coverage list: which DeFi protocols CoinLedger auto-classifies vs. surfaces via PBT.
- Accuracy rate: what fraction of PBT-surfaced transactions the user correctly classifies.
- Whether PBT classifications are reversible and auditable across a multi-session reconciliation.
- Product roadmap for reducing PBT volume via improved auto-classification (LLM-based, per-protocol adapters).
