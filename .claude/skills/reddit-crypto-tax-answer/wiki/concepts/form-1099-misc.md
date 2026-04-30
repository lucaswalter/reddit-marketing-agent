---
title: Form 1099-MISC (Miscellaneous Income)
type: concept
jurisdiction: [US]
created: 2026-04-20
updated: 2026-04-20
tags: [us, irs, 1099, ordinary-income, staking, rewards]
sources: [[coinledger-blog-form-1099-misc-2026-04-20]], [[coinledger-blog-crypto-form-1099-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]]
---

## Definition

US [[irs]] information return used to report miscellaneous ordinary income. For crypto, 1099-MISC is issued by exchanges and protocols when a user receives **≥$600** of ordinary-income-character payments in a tax year — typically Box 3 (other income) [[coinledger-blog-form-1099-misc-2026-04-20]]. The form is designed to track income only; it contains no capital-gain information [[coinledger-blog-form-1099-misc-2026-04-20]].

## Crypto issuance pattern

After Coinbase discontinued 1099-K issuance in 2020 (see [[form-1099-k]]), major US exchanges converged on 1099-MISC for income-character events [[coinledger-blog-crypto-form-1099-2026-04-20]]:
- **Staking rewards** (Coinbase, Kraken pre-SEC-settlement, etc.) — FMV at receipt, reported if ≥$600 aggregate in the year [[coinledger-blog-form-1099-misc-2026-04-20]].
- **Rewards-program income** — Coinbase Learn & Earn, USDC rewards, referral bonuses.
- **Interest-like yield** on CeFi lending products where the platform didn't route through 1099-INT.
- **Airdrops** received through exchange distribution (not all airdrops; platform-specific).

The pattern is consistent across major US centralized exchanges, but the $600 threshold means a large population of stakers with small balances receive no 1099-MISC and must self-report. Unreported small-dollar staking is the highest-volume quiet non-compliance in the US crypto tax base [uncited].

## Reconciliation with the return

1099-MISC Box 3 amounts flow through to **Schedule 1, Line 8** (other income) on Form 1040 [[coinledger-guide-united-states-2026-04-20]]. The corresponding FMV-at-receipt becomes the cost basis of the received crypto; subsequent disposal triggers capital gain/loss reported on [[form-8949]] / Schedule D (see [[staking-rewards]]).

## Why it matters vs. 1099-DA

- **1099-MISC covers income-character events; 1099-DA covers dispositions.** A full-service US exchange in 2026+ issues both for an active customer.
- **Different AUR matching logic.** An unreported 1099-MISC triggers a different IRS [[cp2000]] path than an unreported 1099-DA — the former reads as straight income under-reporting, the latter as capital-gain under-reporting.
- **Basis establishment.** 1099-MISC income sets the future cost basis. Practitioners and software must propagate this into lot tracking, otherwise the downstream disposal will be overtaxed on a $0-basis assumption (see [[missing-cost-basis]]).

## Related wiki pages

- [[form-1099-da]], [[form-1099-k]], [[form-8949]], [[staking-rewards]], [[airdrop-taxation]], [[cp2000]], [[united-states]], [[irs]].

## Primary guidance

- IRC §6041 (information at source for payments of $600+) [primary source not yet ingested].
- Notice 2014-21 (property classification, income on receipt) [primary source not yet ingested].
- Rev. Rul. 2023-14 (staking rewards as income on dominion-and-control) [primary source not yet ingested].

## Gaps

- Per-exchange 1099-MISC issuance matrix (which events each major exchange reports) — not in ingested corpus.
- Treatment of NFT royalty payments: whether 1099-MISC, 1099-NEC, or neither.
- Interaction with 1099-DA for exchanges that issue both: whether staking rewards ever migrate to the 1099-DA box structure.
