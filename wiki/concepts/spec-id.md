---
title: Specific Identification (Spec-ID)
type: concept
jurisdiction: [US, AU, ZA]
created: 2026-04-20
updated: 2026-04-20
tags: [cost-basis, spec-id, hifo, lifo, election]
sources: [[coinledger-guide-united-states-2026-04-20]], [[coinledger-blog-cryptocurrency-tax-calculations-fifo-and-lifo-costing-methods-explained-2026-04-20]], [[coinledger-guide-australia-2026-04-20]], [[coinledger-guide-south-africa-2026-04-20]]
---

## Definition

Specific Identification is a cost-basis method where the taxpayer **nominates the specific lot** being disposed of, as opposed to a formula-driven assignment (FIFO/LIFO/HIFO/ACB). In the US, Spec-ID is the vehicle through which HIFO or LIFO orderings are actually achieved — the IRS permits Spec-ID and allows the taxpayer to select the highest-basis lot (effectively HIFO) or the latest lot (LIFO) if per-lot identification is maintained [[coinledger-guide-united-states-2026-04-20]].

## US mechanics

Per Treas. Reg. §1.1012-1(c) and the IRS crypto FAQ [primary source not yet ingested], Spec-ID for crypto requires:
- **Contemporaneous identification** of the specific unit being disposed of, by date acquired and cost basis, **at or before the time of the sale** [[coinledger-guide-united-states-2026-04-20]].
- **Records** sufficient to substantiate the identification — the wallet, exchange, acquisition transaction, proceeds.
- **Consistency** within a lot-matching engine — you cannot Spec-ID into HIFO on some dispositions and into LIFO on others opportunistically within a wallet without documentation.

In practice, crypto-tax software (CoinLedger and competitors) treats the user's selected method (HIFO, LIFO, Spec-ID custom) as a **Spec-ID election** and generates per-disposal lot-matching records that satisfy the contemporaneous-documentation requirement [[coinledger-blog-cryptocurrency-tax-calculations-fifo-and-lifo-costing-methods-explained-2026-04-20]]. The IRS has not challenged this interpretation in any ingested source.

## Why HIFO/LIFO are actually Spec-ID

HIFO and LIFO are not independently authorized methods in the US — they are **outcome labels** for a specific Spec-ID policy [[coinledger-guide-united-states-2026-04-20]]:
- **HIFO** = Spec-ID with "always pick the highest-basis lot" policy.
- **LIFO** = Spec-ID with "always pick the most recent lot" policy.
- **Custom Spec-ID** = user-selected lots (e.g., select long-term lots to lock in LTCG rate).

If a taxpayer cannot maintain per-lot records, the fallback is **FIFO**.

## Documentation requirements

The contemporaneous-identification requirement is lightly enforced in practice, but a well-resourced audit can challenge it. Defensible records include [[coinledger-guide-united-states-2026-04-20]]:
- Exchange transaction exports with timestamps and per-lot IDs.
- Wallet addresses and TXIDs on-chain.
- Crypto-tax software audit trail showing the lot-selection policy applied at each disposal.
- Per-lot cost basis schedule with acquisition dates.

Post-Rev-Proc-2024-28, per-wallet accounting (see [[per-wallet-cost-basis]]) makes Spec-ID cleaner — the universe of eligible lots at each wallet is narrower, and the exchange 1099-DA will eventually report basis per lot.

## Variance across jurisdictions

- **Australia (investors):** Individual identification permitted → HIFO/LIFO/FIFO all available [[coinledger-guide-australia-2026-04-20]]. Australia traders: FIFO only [[coinledger-guide-australia-2026-04-20]].
- **South Africa:** Spec-ID inferred from SARS stock guidance (no explicit crypto rule) [[coinledger-guide-south-africa-2026-04-20]].
- **UK, Canada, Sweden, Germany, Spain, Denmark, Ireland:** Spec-ID **not** available — forced into pooling/averaging/FIFO (see [[cost-basis-methods]]).

## Practitioner implications

- **Spec-ID is the only path to HIFO for US crypto.** If a user wants minimum-gain lot matching, the software invocation is effectively a Spec-ID election with HIFO policy.
- **Method consistency.** Changing from FIFO to HIFO/LIFO mid-year without supporting Spec-ID documentation is audit-vulnerable.
- **Per-wallet narrowing.** Post-2025, Spec-ID operates within a wallet's lot set, not across the universal pool (see [[per-wallet-cost-basis]]).
- **1099-DA interaction.** Exchanges reporting basis on 1099-DA generally apply FIFO at the exchange level. A taxpayer using Spec-ID/HIFO will have basis figures that differ from the 1099-DA — the remedy is filing [[form-8949]] with correct basis and accepting [[cp2000]] risk.

## Related wiki pages

- [[cost-basis-methods]], [[per-wallet-cost-basis]], [[tax-loss-harvesting]], [[form-8949]], [[form-1099-da]], [[cp2000]], [[united-states]], [[australia]].

## Primary guidance

- Treas. Reg. §1.1012-1(c) [primary source not yet ingested].
- IRS Crypto FAQs [primary source not yet ingested].
- Rev. Proc. 2024-28 (per-wallet overlay) [primary source not yet ingested].

## Gaps

- Official IRS position on blanket HIFO elections without per-disposal Spec-ID paperwork.
- Audit rate and outcomes for Spec-ID/HIFO elections — not in ingested corpus.
- Treatment of Spec-ID when crypto is on-chain without exchange-level transaction IDs.
