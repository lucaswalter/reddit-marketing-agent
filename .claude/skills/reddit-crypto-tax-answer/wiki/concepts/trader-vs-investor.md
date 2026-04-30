---
title: Trader vs investor classification
type: concept
jurisdiction: [US, AU, IE, ZA, UK]
created: 2026-04-20
updated: 2026-04-20
tags: [classification, trader, investor, business-income, capital-gains]
sources: [[coinledger-guide-united-states-2026-04-20]], [[coinledger-guide-australia-2026-04-20]], [[coinledger-guide-ireland-2026-04-20]], [[coinledger-guide-south-africa-2026-04-20]], [[coinledger-guide-united-kingdom-2026-04-20]], [[coinledger-guide-canada-2026-04-20]]
---

## Definition

The classification of a crypto market participant as a **trader** (carrying on a business / trading activity) vs an **investor** (holding capital assets for appreciation). The classification is load-bearing: it determines whether gains are **capital gains** (often preferentially taxed) or **ordinary / business income** (always at full marginal rates), whether expenses are deductible, whether losses offset other income, and what cost-basis method options are available.

## Variance across jurisdictions

| Jurisdiction | Test | Implication if classified as trader |
|---|---|---|
| **US** | §475 mark-to-market **election** (limited to trader-in-securities status via IRC §475(f)) — crypto eligibility contested | §475(f) MTM election: ordinary-income treatment year-end, no wash-sale rule regardless, losses fully deductible [[coinledger-guide-united-states-2026-04-20]] |
| **Australia** | ATO trader-vs-investor facts test: volume, organization, profit-motive | Trader: ordinary income, **no 50% CGT discount**, FIFO only — materially worse outcome for gains [[coinledger-guide-australia-2026-04-20]] |
| **Ireland** | "Badges of Trade" test (volume, frequency, organization, motive) | Income-tax treatment instead of 33% CGT; 20/40% marginal rates can exceed or fall below CGT depending on level [[coinledger-guide-ireland-2026-04-20]] |
| **South Africa** | SARS case-by-case: motive (long-term growth vs short-term profit), frequency, holding period | **Max effective CGT ~18% vs max income tax 45%** — single largest rate delta of ingested jurisdictions [[coinledger-guide-south-africa-2026-04-20]] |
| **UK** | HMRC CRYPTO20250 — business vs hobby test; genuine "trader" status rare | Trader: income tax (up to 45%) instead of 18/24% CGT. Losses against other income if trading [[coinledger-guide-united-kingdom-2026-04-20]] |
| **Canada** | CRA business-vs-capital test (frequency, knowledge, time spent, financing) | 100% income inclusion vs. 50% capital inclusion. Business losses offset all income [[coinledger-guide-canada-2026-04-20]] |

## US: the §475(f) election

IRC §475(f) allows a taxpayer who qualifies as a **trader in securities** to elect **mark-to-market** treatment [primary source not yet ingested]:
- Year-end unrealized gains/losses recognized as ordinary.
- No §1091 wash-sale rule.
- Losses fully deductible against ordinary income (no $3K cap).
- Election must be made by the prior year's return filing date (April 15) — a meaningful trap.

**Crypto eligibility is unresolved.** §475(f) references "securities" — the same scope issue that keeps crypto out of §1091 wash-sale (see [[wash-sale-rule]]). The IRS has not issued guidance explicitly extending or denying §475(f) MTM to crypto traders, and the ingested corpus doesn't resolve it [[coinledger-guide-united-states-2026-04-20]]. Aggressive practitioners take the election for active crypto-focused traders; the conservative view is that §475(f) is not available for crypto-only traders.

Related: the §162 trade-or-business deduction and Schedule C treatment are separate from §475 — a full-time crypto trader may deduct ordinary business expenses without electing MTM [[coinledger-guide-united-states-2026-04-20]].

## Australia: the highest-stakes case

The AU regime makes trader-vs-investor **more consequential** than any other OECD jurisdiction in the ingested corpus. An investor holding >12 months gets a **50% CGT discount** [[coinledger-guide-australia-2026-04-20]]; a trader gets none. The ATO facts-test (volume, business-like organization, profit motive, capital available) is applied without safe harbor. A single high-volume year can re-characterize.

## Ireland and South Africa: the Badges of Trade lineage

Both IE and ZA apply variants of the common-law **Badges of Trade** test inherited from UK case law [primary source not yet ingested]. The test is not a bright line — it's a multi-factor analysis:
- Subject matter of the transaction (divisible units vs. single large asset)
- Length of ownership
- Frequency of similar transactions
- Supplementary work (modification, marketing)
- Circumstances of sale
- Motive

In ZA, lacking a 3-year investor-safe-harbor for crypto [[coinledger-guide-south-africa-2026-04-20]], the classification is especially unstable.

## Why it's a high-stakes classification

- **Rate delta.** 50% AU CGT discount, 33% IE flat CGT, 18% ZA effective CGT vs. full marginal ordinary rates — the gap can be 15–30 percentage points.
- **No election in most jurisdictions.** AU/IE/ZA/UK don't let you choose — the taxonomy is determined by activity. US §475(f) is unusual in being electable.
- **Audit vulnerability.** A taxpayer who files as investor while trading at business-like scale invites reclassification plus penalties. The reverse (trader filing) is usually accepted if elections are timely.
- **Software implication.** Reporting rails differ: Schedule C vs Schedule D (US), Question 2 vs Section 18 (AU), Form 11 vs Form CG1 (IE).

## Related wiki pages

- [[wash-sale-rule]], [[cost-basis-methods]], [[tax-loss-harvesting]], [[united-states]], [[australia]], [[ireland]], [[south-africa]], [[united-kingdom]], [[canada]].

## Primary guidance

- **US:** IRC §475(f); IRC §162; Commissioner v. Groetzinger (trader-in-securities criteria) [primary source not yet ingested].
- **AU:** ATO crypto-investor vs. trader guidance [primary source not yet ingested].
- **IE/UK:** Badges of Trade — case law, HMRC CRYPTO20250 [primary source not yet ingested].

## Gaps

- No ingested source explicitly confirms or denies §475(f) crypto eligibility.
- Volume/frequency thresholds that tip ATO classification are not quantified.
- Interaction with TFSA/SMSF/IRA structures — trader classification inside these is usually disregarded but mechanics vary.
