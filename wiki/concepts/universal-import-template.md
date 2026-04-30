---
title: Universal Import Template — CoinLedger product concept
type: concept
jurisdiction: [global]
created: 2026-04-20
updated: 2026-04-20
tags: [coinledger-product, csv-import, data-ingestion]
sources: [[coinledger-help-6028758-universal-manual-import-template-guide-2026-04-20]], [[coinledger-help-6173382-import-transactions-from-a-partially-supported-exchange-with-the-universal-import-template-csv-file-2026-04-20]], [[coinledger-help-4998740-troubleshooting-manual-csv-file-import-failures-due-to-incorrect-formatting-2026-04-20]]
---

## Definition

The **Universal Import Template** is CoinLedger's canonical CSV schema for manual transaction ingestion from any source — used when an exchange or wallet is (a) not supported by a dedicated integration, (b) partially supported and missing some transaction types, or (c) producing exports CoinLedger can't parse natively [[coinledger-help-6028758-universal-manual-import-template-guide-2026-04-20]]. It is the product's escape hatch for long-tail and unsupported venues.

The template is the contract between user data and the CoinLedger ingestion engine: conforming CSVs are ingested deterministically; non-conforming CSVs fail with formatting-error diagnostics [[coinledger-help-4998740-troubleshooting-manual-csv-file-import-failures-due-to-incorrect-formatting-2026-04-20]].

## The CSV contract

Per [[coinledger-help-6028758-universal-manual-import-template-guide-2026-04-20]], the template defines a fixed column set. While the help articles summarize rather than enumerate every field, the canonical required and optional columns (from the help-center article structure):

**Required columns** [uncited — the help-article body is summarized in the source page but specific column names aren't in the TL;DR]:
- Date / timestamp (specific format).
- Transaction type (from accepted enum).
- Incoming asset and quantity.
- Outgoing asset and quantity.
- Source / destination identifier.

**Optional columns**:
- Fee asset and amount.
- USD value at time of transaction (for price override).
- Transaction hash / external ID.
- Notes / description.

The help article on partial-exchange imports [[coinledger-help-6173382-import-transactions-from-a-partially-supported-exchange-with-the-universal-import-template-csv-file-2026-04-20]] describes the workflow where a user combines CoinLedger's native API pull with a Universal-template CSV for transaction types the API didn't cover.

## Accepted transaction types

Per help center conventions (drawn from the transaction-type enum referenced across multiple help articles [uncited — specific list not in TL;DR of the source pages]):
- **Buy / Sell** — crypto-for-fiat.
- **Trade** — crypto-for-crypto.
- **Deposit / Withdrawal** — transfer in/out of the platform (non-taxable).
- **Income** — generic ordinary income (staking, interest, referral, airdrop with explicit receipt basis).
- **Mining** — ordinary income with FMV at receipt.
- **Staking** — ordinary income at FMV.
- **Airdrop** — ordinary income at FMV.
- **Gift Sent / Received** — jurisdiction-specific handling.
- **Lost / Stolen** — potential deductible loss (jurisdiction-dependent).
- **Spend** — crypto used for goods/services (disposal).

## Common failure modes

From [[coinledger-help-4998740-troubleshooting-manual-csv-file-import-failures-due-to-incorrect-formatting-2026-04-20]]:
- Date-format mismatch (region-specific DD/MM vs. MM/DD).
- Unrecognized transaction type (typos, unknown enum value).
- Currency ticker typos (BTC vs. XBT, stablecoin variants).
- Numeric formatting (European comma decimal vs. US period).
- Missing required columns.
- Row count or encoding issues (non-UTF8, Excel serialization artifacts).

## Why it matters

- **Coverage floor.** CoinLedger's native integrations cover a large but finite set (91 exchanges, 22 wallets, 51 chains per the help-center inventory). The Universal template extends coverage to anything with a CSV export — otherwise uncoverable venues become coverable.
- **User-last-resort for reconciliation.** When an automated integration fails partway through history or drops transaction types, the Universal template fills the gap.
- **Data-quality choke point.** Manual CSV imports are the largest source of user-side data-integrity issues — typos, dupes, and misclassifications propagate straight to [[missing-cost-basis]] warnings and bad basis figures on [[form-8949]].
- **Competitor parity.** Every crypto-tax platform has a CSV template; comparison reveals how constrained or flexible CoinLedger's is. The Universal template's breadth is a competitive feature for users with obscure-venue history.

## Related wiki pages

- [[missing-cost-basis]], [[potential-bridges-trades-transfers]], [[form-8949]], [[coinledger]].

## Primary guidance

- Not applicable — product-internal schema.

## Gaps

- Full column schema not in TL;DRs — requires raw-file read for complete spec.
- Comparison to competitor schemas (Koinly, CoinTracker, TokenTax generic CSVs).
- Template versioning history — when columns or enum values have changed.
- Whether failed-import rows are recoverable via retry or require a fresh upload.
