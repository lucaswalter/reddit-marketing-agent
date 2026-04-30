---
title: Germany
type: jurisdiction
created: 2026-04-20
updated: 2026-04-20
tags: [germany, eu, bmf, bzst]
sources: [[coinledger-homepage-2026-04-20]], [[coinledger-guide-germany-2026-04-20]]
---

## Why this page matters

[[coinledger]] explicitly calls out "Built For Germany Tax Rules" as a homepage feature [[coinledger-homepage-2026-04-20]] — the only non-US jurisdiction with dedicated page-level product logic. Germany's 1-year tax-free holding rule is the feature that makes generic cost-basis-only logic insufficient. Lots must be tracked with acquisition dates to determine taxability.

## Classification

Crypto is "other economic goods" (*sonstiges Wirtschaftsgut*) under §23 EStG — a **private-sales** regime, not a capital-gains-tax regime [[coinledger-guide-germany-2026-04-20]].

## Tax treatment by transaction type

- **Dispositions <12 months:** Short-term gain taxed at ordinary income rates (subject to €600/year exemption) [[coinledger-guide-germany-2026-04-20]].
- **Dispositions >12 months:** **Fully tax-free** for individuals. Signature German feature [[coinledger-guide-germany-2026-04-20]].
- **Mining:** Income at FMV on receipt. Business deducts expenses; hobby miners cannot [[coinledger-guide-germany-2026-04-20]].
- **Staking:** Income at FMV on receipt. Capital gain on disposal (tax-free if >12mo) [[coinledger-guide-germany-2026-04-20]].
- **Airdrops:** Taxable income only if recipient took action (gas, social post) to claim. Passive airdrops tax-free on receipt [[coinledger-guide-germany-2026-04-20]].
- **Hard forks:** New coins not taxable on receipt. Taxed if disposed within 12 months [[coinledger-guide-germany-2026-04-20]].
- **NFTs:** No explicit BMF guidance; guide applies 12-month rule by analogy. Creator revenue = income [[coinledger-guide-germany-2026-04-20]].
- **DeFi:** No explicit BMF guidance. Guide assumes: yield is income; disposals follow 12-month rule [[coinledger-guide-germany-2026-04-20]].
- **Stablecoins:** Same 12-month rule — disposal in <12mo is taxable event [[coinledger-guide-germany-2026-04-20]].
- **Gifts:** Tax-free up to €20,000 for friends, €500,000 for spouses. Above threshold: gift tax 7–50% [[coinledger-guide-germany-2026-04-20]].
- **Compensation in crypto:** Ordinary income [[coinledger-guide-germany-2026-04-20]].

## Rates and thresholds

- **Income tax (2024):** 0% ≤€10,908 / 14–42% progressive band / 42% above €62,810 / 45% above €277,826. Plus 5.5% solidarity surcharge for earners >€10,908 [[coinledger-guide-germany-2026-04-20]].
- **Short-term gain exemption:** €600/yr on short-term private-sale gains below which no tax/filing [[coinledger-guide-germany-2026-04-20]].
- **Long-term:** 0% (fully exempt) [[coinledger-guide-germany-2026-04-20]].

## Cost basis method

- **FIFO** is the preferred method [[coinledger-guide-germany-2026-04-20]].
- Per-wallet lot tracking with acquisition dates is essential given the 12-month rule.

## Reporting forms and deadlines

- **Hauptformular ESt 1 A** (general income declaration) + **Anlage SO** (other income, including short-term private-sale crypto gains) [[coinledger-guide-germany-2026-04-20]].
- Filed online via **Elster** (Elektronische Steuererklärung) — the BZSt portal.
- **Deadline:** July 31 of the year following the calendar tax year [[coinledger-guide-germany-2026-04-20]].
- Late penalty: 0.25%/month of unpaid tax, capped ~€25K.

## Losses

- Short-term crypto losses offset short-term crypto gains [[coinledger-guide-germany-2026-04-20]].
- **Long-term "losses" (held >12mo) are not deductible** — symmetric to long-term gains being tax-free. Meaningful planning implication: never hold losing positions past the 12-month mark if you want a deductible loss.
- No wash-sale equivalent addressed in source.

## Regulator and primary guidance

- Operational regulator: [[bzst]] (Bundeszentralamt für Steuern) — handles tracking, filing, Elster portal.
- Policy regulator: BMF (Bundesministerium der Finanzen) — issues interpretive guidance. 2022 BMF letter clarified staking/lending treatment (10-year extension dropped, back to 1 year).

## Notable quirks

- **1-year tax-free holding rule** — the defining German crypto-tax feature. Makes acquisition-date lot tracking load-bearing in ways most jurisdictions don't require.
- **Passive-airdrop tax-free treatment** — unusual and investor-friendly among OECD regimes [[coinledger-guide-germany-2026-04-20]].
- **Symmetric long-term treatment** — long-term gains tax-free, long-term losses undeductible.
- **Solidarity surcharge** (5.5%) stacks on top of income tax above threshold [[coinledger-guide-germany-2026-04-20]].

## Enforcement

- EU 6th AMLD (Dec 2020) required EU-wide exchange registration.
- **DAC8 live January 2026** — CASPs must report domestic and cross-border transactions to tax authorities [[coinledger-guide-germany-2026-04-20]].

## Products serving Germany

- [[coinledger]] "Built For Germany Tax Rules" [[coinledger-homepage-2026-04-20]]
- Koinly (strong German presence), Blockpit (Austrian but covers DE) — entity pages not yet created

## Gaps

- Exact BMF guidance dates and citations (2022 BMF letter on staking/lending).
- DAC8 implementation specifics.
- Per-wallet vs universal FIFO treatment under German rules.
- NFT creator-royalty tax treatment.
- Treatment of margin/futures.
- Recent case law on the 1-year rule and abuse prevention.
