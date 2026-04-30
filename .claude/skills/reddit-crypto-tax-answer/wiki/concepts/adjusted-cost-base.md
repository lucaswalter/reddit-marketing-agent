---
title: Adjusted Cost Base (Canada)
type: concept
jurisdiction: [CA]
created: 2026-04-20
updated: 2026-04-20
tags: [canada, cra, cost-basis, average-cost]
sources: [[coinledger-guide-canada-2026-04-20]]
---

## Definition

**Adjusted Cost Base (ACB)** is Canada's **mandatory** cost-basis method for identical properties — including cryptocurrency [[coinledger-guide-canada-2026-04-20]]. ACB is a running weighted average: every acquisition recomputes the per-unit cost across all held units of the same asset. No FIFO / LIFO / HIFO / Spec-ID election is permitted. CRA applies this to crypto by treating each cryptocurrency as "identical property" [[coinledger-guide-canada-2026-04-20]].

Statutory source: Income Tax Act s.47 ("identical properties") [primary source not yet ingested].

## Mechanics

**ACB per unit = (Σ cumulative acquisition cost + adjustments) / (Σ units held).**

Each buy:
- New total cost = prior total cost + buy cost.
- New unit count = prior unit count + buy units.
- New ACB = new total cost / new unit count.

Each sell:
- Cost basis used = current ACB × units sold.
- Total cost is reduced proportionally (cost basis removed equals units sold × ACB at disposal).
- Remaining ACB per unit is unchanged.

Worked example: Buy 1 BTC at CAD $40K. Buy 1 BTC at CAD $60K. ACB = (40+60)/2 = $50K/BTC. Sell 1 BTC at $80K → gain = $80K − $50K = $30K, of which 50% ($15K) is included in taxable income per Canada's 50% capital gains inclusion [[coinledger-guide-canada-2026-04-20]]. Remaining: 1 BTC with ACB $50K.

## Superficial Loss interaction

When a disposal triggers the Superficial Loss Rule (see [[superficial-loss-rule]]), the disallowed loss is **added to the ACB** of the reacquired property — deferring the loss as a basis increase rather than realizing it [[coinledger-guide-canada-2026-04-20]]. This is the cleanest illustration of how Canada's framework treats disallowed losses as basis adjustments rather than permanent disallowances.

## Differences from US/UK/AU

- **US:** FIFO default with Spec-ID/HIFO/LIFO election (see [[cost-basis-methods]], [[spec-id]]).
- **UK:** Section 104 pool — structurally similar to ACB (also average cost) but with the Same Day + 30-day B&B matching rules running before the pool (see [[shared-pool-accounting]], [[bed-and-breakfast-rule]]).
- **AU:** Investors can elect FIFO/LIFO/HIFO via individual identification (see [[cost-basis-methods]]).
- **Canada:** **No election.** ACB is mandatory.

The UK and Canada both force averaging, but the UK's matching-order overlay makes them functionally different: a UK taxpayer's pool doesn't capture same-day/30-day reacquisitions, whereas the Canadian ACB does, and the Canadian superficial-loss adjustment then re-adds the disallowed loss to ACB.

## Fees and adjustments

ACB includes acquisition costs (exchange fees, network fees incurred to acquire) and is reduced by non-disposal cost recoveries. Practical CoinLedger-relevant points [[coinledger-guide-canada-2026-04-20]]:
- **Transfer fees paid in crypto** are themselves taxable disposals of the fee crypto and do not add to the receiving asset's ACB.
- **Mining/staking rewards (CA individual, hobby):** $0 ACB per CRA guidance for individuals; income at FMV only arises for businesses.
- **Hard forks (individual):** $0 ACB on the new coin; CGT on subsequent disposal.
- **Airdrops (individual):** Treated similarly — $0 ACB, CGT on disposal.

## Why it matters

- **No HIFO.** A Canadian high-basis taxpayer cannot elect into HIFO to minimize a gain — the average is the average.
- **Year-over-year software continuity.** A user migrating crypto-tax platforms mid-history must carry full ACB state across the migration. CoinLedger and competitors that build per-country logic need ACB engines distinct from US FIFO engines.
- **50% inclusion applies to losses too** [[coinledger-guide-canada-2026-04-20]]. Only half a capital loss offsets capital gains — a structural quirk of Canada's inclusion regime.
- **ACB can exceed CAD-purchase cost via crypto-acquired-from-crypto flows.** Receiving BTC via a crypto-to-crypto trade sets ACB to the FMV of the received BTC (equal to the disposed crypto's proceeds value in CAD).

## Related wiki pages

- [[superficial-loss-rule]], [[cost-basis-methods]], [[shared-pool-accounting]], [[canada]], [[cra]].

## Primary guidance

- Income Tax Act s.47 (identical properties) [primary source not yet ingested].
- CRA Guide for Cryptocurrency Users and Tax Professionals [primary source not yet ingested].
- CRA T4037 Capital Gains guide [primary source not yet ingested].

## Gaps

- Detailed ACB worked examples for mining-as-business disposals (how ACB transitions between business-income coin and capital-asset coin).
- Treatment of wrapped tokens (WBTC vs BTC) as "identical property" — CRA silent.
- ACB behavior across self-custody wallets and exchanges (Canada hasn't adopted a per-wallet rule analogous to US Rev. Proc. 2024-28).
