---
title: Bed and Breakfast Rule (UK 30-day, SA 45-day)
type: concept
jurisdiction: [UK, ZA]
created: 2026-04-20
updated: 2026-04-20
tags: [uk, hmrc, south-africa, sars, wash-sale, matching-order]
sources: [[coinledger-guide-united-kingdom-2026-04-20]], [[coinledger-guide-south-africa-2026-04-20]]
---

## Definition

"Bed and Breakfasting" describes the historical UK practice of selling at year-end (the "bed") and rebuying the next morning (the "breakfast") to realize a capital loss or use the annual CGT exemption while retaining the position. The Bed and Breakfast Rule is the statutory anti-abuse matching rule that neutralizes this by forcing disposal-side matching against reacquisitions within a fixed window [[coinledger-guide-united-kingdom-2026-04-20]].

Two flavors in the ingested corpus:
- **UK: 30-day window**, applies to all chargeable assets including crypto [[coinledger-guide-united-kingdom-2026-04-20]].
- **South Africa: 45-day window** for the same-asset rule [[coinledger-guide-south-africa-2026-04-20]].

## UK mechanics

The UK matching order for crypto disposals [[coinledger-guide-united-kingdom-2026-04-20]]:

1. **Same Day Rule:** match disposals against same-day acquisitions first.
2. **30-day Bed & Breakfast Rule:** match against acquisitions of the same asset within 30 days **after** the disposal.
3. **Section 104 pool:** remainder matches against the pool's average cost (see [[shared-pool-accounting]]).

Note the asymmetry vs. Canada's superficial loss: the UK rule only looks **forward** (30 days after). Acquisitions in the 30 days *before* the disposal don't trigger — they go into the Section 104 pool normally. US §1091 and Canada's superficial loss look both ways; UK B&B is post-disposal only [uncited — derived from the HMRC matching order].

Effect: UK taxpayer sells 1 BTC at a loss on Dec 31; rebuys 1 BTC on Jan 5. The disposal matches against the Jan 5 buy, not the Section 104 pool. The realized loss/gain is calculated against the actual Jan 5 cost, typically near-zero (same asset, few days apart). The anti-abuse goal is achieved: the year-end loss harvest fails.

## SA 45-day mechanics

SARS applies a longer, 45-day window for the same-asset reacquisition rule [[coinledger-guide-south-africa-2026-04-20]]. This is **stricter than the UK's 30-day** and among the widest anti-wash windows globally. The SA rule is informally called the "Bed and Breakfast Rule" in the CoinLedger guide despite operating slightly differently from the UK original.

The SA rule interacts with the trader-vs-investor classification (see [[trader-vs-investor]]) — for traders operating under income-tax rather than CGT, the 45-day window doesn't disallow losses in the same way (business losses follow different rules).

## Interaction with other UK rules

Because UK B&B operates within Section 104 pooling and alongside the Same Day Rule, the matching sequence resolves edge cases deterministically:

- **Same-day buy AND >Section 104 pool AND 30-day reacquisition:** Same-day buy is matched first (consuming those units), then the 30-day B&B rule applies to any remaining disposal, then the pool absorbs the rest.
- **Multiple 30-day reacquisitions:** Matched chronologically — earliest reacquisition first.

## Why it matters

- **UK tax-loss harvesting is structurally disabled** for same-asset sell-rebuy tactics. To realize a crypto loss and re-establish exposure, a UK user must (a) wait 30 days, (b) buy a non-identical asset as proxy, or (c) use a spouse transfer (spouse gifts are outside CGT and the B&B matching doesn't extend to spouse) [[coinledger-guide-united-kingdom-2026-04-20]].
- **Annual CGT exemption (£3,000) erosion.** Pre-B&B, users could "bed-and-breakfast" to reset basis at year-end and use the annual exemption against the crystallized gain. Post-B&B, this is blocked.
- **Software implication.** Any tax platform serving UK users needs matching-order logic — naive FIFO on crypto UK data produces wrong outputs.

## Related wiki pages

- [[shared-pool-accounting]], [[wash-sale-rule]], [[superficial-loss-rule]], [[tax-loss-harvesting]], [[cost-basis-methods]], [[united-kingdom]], [[south-africa]], [[hmrc]], [[sars]].

## Primary guidance

- **UK:** TCGA 1992 s.106A (B&B matching for cryptoassets) [primary source not yet ingested].
- **UK:** HMRC Cryptoassets Manual matching-rule sections [primary source not yet ingested].
- **SA:** SARS Crypto FAQs, reviewed 23 June 2021 [primary source not yet ingested].

## Gaps

- Whether UK HMRC B&B applies to DeFi-protocol acquisitions (e.g., LP withdrawal creating a "new" BTC position) — not explicitly addressed.
- SA 45-day rule mechanics (exact matching sequence vs UK parallels) not spelled out in ingested corpus.
- Spouse transfer treatment under SA B&B rule.
