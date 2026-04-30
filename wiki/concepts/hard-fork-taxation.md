---
title: Hard-fork taxation (cross-jurisdictional)
type: concept
jurisdiction: [US, CA, AU, DE, UK, NZ]
created: 2026-04-20
updated: 2026-04-20
tags: [hard-fork, ordinary-income, capital-gains, cross-jurisdictional]
sources: [[coinledger-blog-how-are-cryptocurrency-hard-forks-taxed-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]], [[coinledger-guide-germany-2026-04-20]], [[coinledger-guide-canada-2026-04-20]], [[coinledger-guide-australia-2026-04-20]], [[coinledger-guide-united-kingdom-2026-04-20]], [[coinledger-guide-new-zealand-2026-04-20]]
---

## Definition

A **hard fork** is a permanent, non-backward-compatible divergence in a blockchain protocol resulting in two distinct chains [[coinledger-blog-how-are-cryptocurrency-hard-forks-taxed-2026-04-20]]. Holders at the fork block typically receive the new-chain token 1:1 (canonical example: Bitcoin Cash from Bitcoin, August 1, 2017) [[coinledger-blog-how-are-cryptocurrency-hard-forks-taxed-2026-04-20]]. **Soft forks** maintain compatibility and create no new asset — not taxable in any ingested jurisdiction.

## Variance across jurisdictions

| Jurisdiction | Treatment on receipt | Basis | Disposal |
|---|---|---|---|
| **US** | Ordinary income at FMV on receipt when dominion-and-control established | FMV at receipt | Capital gain/loss vs. basis [[coinledger-guide-united-states-2026-04-20]] |
| **Canada (individual)** | Not taxable on receipt | $0 | Full-proceeds capital gain on disposal [[coinledger-guide-canada-2026-04-20]] |
| **Canada (business)** | Ordinary income at FMV on receipt | FMV at receipt | Income on subsequent disposal [[coinledger-guide-canada-2026-04-20]] |
| **Australia** | Not taxable on receipt | $0 cost base | Full-proceeds CGT on disposal [[coinledger-guide-australia-2026-04-20]] |
| **Germany** | Not taxable on receipt | $0 | §23 EStG: taxable as short-term private sale if disposed <12mo after receipt; tax-free if held >12mo [[coinledger-guide-germany-2026-04-20]] |
| **UK** | Guide does not explicitly cover; likely treated like passive airdrop (no income on receipt, CGT on disposal) [[coinledger-guide-united-kingdom-2026-04-20]] | $0 or apportioned from original pool [uncited] | CGT on disposal |
| **Denmark** | $0 cost basis; full proceeds treated as ordinary income on disposal [[coinledger-guide-denmark-2026-04-20]] | $0 | Income on disposal |
| **New Zealand** | Generally **not taxable on receipt** (exceptions: crypto business, profit-making scheme, acquired-for-disposal). Unusual among OECD regimes [[coinledger-guide-new-zealand-2026-04-20]] | $0 (or FMV if income-triggered) | Income on disposal |

## US: the Rev. Rul. 2019-24 doctrine

The IRS's position was codified in **Rev. Rul. 2019-24** [primary source not yet ingested]: a hard fork producing new cryptocurrency generates **ordinary income** at FMV on the date the taxpayer achieves **dominion and control** (i.e., can transfer, sell, exchange, or otherwise dispose) [[coinledger-guide-united-states-2026-04-20]]. Pre-ruling, the Bitcoin Cash fork had been the canonical uncertainty case; Rev. Rul. 2019-24 retroactively clarified [[coinledger-blog-how-are-cryptocurrency-hard-forks-taxed-2026-04-20]].

Key interpretive question: when is dominion-and-control established? If an exchange holds the old coin and doesn't support the new chain until months later, receipt is deferred. Self-custody with software support is generally immediate. No ingested source gives a bright-line rule.

## Why the variance matters

- **Timing asymmetry.** US taxpayers owe tax at fork time regardless of whether they dispose; AU/CA individuals only owe on disposal. For a large fork into a token that subsequently crashes, the US taxpayer can end up with a phantom income bill no disposal repays.
- **Basis planning.** US $0-basis cases don't exist on hard forks (unlike AU/CA) — basis equals FMV at receipt.
- **German 1-year rule applies to received coin.** The 12-month holding clock starts at receipt; hold >12 months → tax-free disposal [[coinledger-guide-germany-2026-04-20]].
- **NZ's passive treatment** is a genuine outlier and merits its own entity page on the IRD position.

## Related wiki pages

- [[airdrop-taxation]], [[staking-rewards]], [[united-states]], [[canada]], [[australia]], [[germany]], [[united-kingdom]], [[new-zealand]], [[denmark]].

## Primary guidance

- **US:** Rev. Rul. 2019-24; Notice 2014-21 [primary source not yet ingested].
- **Canada:** CRA Guide for Cryptocurrency Users [primary source not yet ingested].
- **Germany:** §23 EStG; BMF letter of 2022 [primary source not yet ingested].
- **UK:** HMRC Cryptoassets Manual CRYPTO22000 series [primary source not yet ingested].
- **New Zealand:** IRD crypto-asset guidance pages [primary source not yet ingested].

## Gaps

- UK HMRC explicit hard-fork guidance not surfaced in ingested corpus [[coinledger-guide-united-kingdom-2026-04-20]].
- Ireland hard-fork treatment not in ingested guide [[coinledger-guide-ireland-2026-04-20]].
- Spain AEAT hard-fork position.
- Treatment where the fork produces tokens the holder cannot practically access (unsupported exchange, lost keys to pre-fork wallet).
