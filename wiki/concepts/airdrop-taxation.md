---
title: Airdrop taxation (cross-jurisdictional)
type: concept
jurisdiction: [US, UK, DE, ES, AU, CA, NZ]
created: 2026-04-20
updated: 2026-04-20
tags: [airdrop, ordinary-income, cross-jurisdictional]
sources: [[coinledger-blog-airdrop-taxes-2026-04-20]], [[coinledger-blog-uniswap-airdrop-taxes-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]], [[coinledger-guide-united-kingdom-2026-04-20]], [[coinledger-guide-germany-2026-04-20]], [[coinledger-guide-spain-2026-04-20]], [[coinledger-guide-australia-2026-04-20]], [[coinledger-guide-canada-2026-04-20]], [[coinledger-guide-new-zealand-2026-04-20]]
---

## Definition

An **airdrop** is a free distribution of tokens to wallet addresses, typically for marketing, community-building, or protocol-ownership bootstrapping [[coinledger-blog-airdrop-taxes-2026-04-20]]. Canonical example: Uniswap's September 2020 distribution of 400 UNI to each historical user address [[coinledger-blog-airdrop-taxes-2026-04-20]].

## The active-vs-passive distinction

Several jurisdictions condition taxability on whether the recipient **took action** to claim the airdrop:

| Jurisdiction | Active airdrop (user action: claim tx, social post, gas paid) | Passive airdrop (unsolicited receipt) |
|---|---|---|
| **US** | Ordinary income at FMV on receipt | Ordinary income at FMV on receipt — IRS doesn't distinguish [[coinledger-guide-united-states-2026-04-20]], [[coinledger-blog-airdrop-taxes-2026-04-20]] |
| **Germany** | Taxable income on receipt | **Tax-free on receipt** — unusually investor-friendly [[coinledger-guide-germany-2026-04-20]] |
| **UK** | Miscellaneous income on receipt (if received in exchange for service/action) | Not income on receipt; CGT on disposal [[coinledger-guide-united-kingdom-2026-04-20]] |
| **Spain** | Likely income at FMV (no explicit AEAT guidance) | Same — AEAT hasn't distinguished [[coinledger-guide-spain-2026-04-20]] |
| **Canada (individual)** | Likely income if tied to service; CGT on disposal if treated as new-asset acquisition | Likely $0-basis new-asset treatment; CGT on disposal [[coinledger-guide-canada-2026-04-20]] |
| **Canada (business)** | Income at FMV | Income at FMV [[coinledger-guide-canada-2026-04-20]] |
| **Australia** | Income at FMV on receipt (ATO explicit) | Income at FMV [[coinledger-guide-australia-2026-04-20]] |
| **New Zealand** | Income on disposal if: crypto business, profit-scheme, service-for-airdrop, acquired-for-disposal | Passive airdrops may escape income treatment [[coinledger-guide-new-zealand-2026-04-20]] |

## US treatment

The IRS position: airdrops are ordinary income at FMV on receipt when dominion-and-control is established [[coinledger-guide-united-states-2026-04-20]]. The logic parallels the Rev. Rul. 2019-24 hard-fork doctrine (see [[hard-fork-taxation]]). Subsequent disposal triggers capital gain/loss vs. basis = FMV-at-receipt. Reported on Schedule 1, Line 8 via [[form-1099-misc]] if ≥$600 from a US exchange issuer.

Practitioner ambiguity: **retroactive airdrops to historical users** (Uniswap-style) create valuation problems when the token has no pre-claim trading market — FMV at "receipt" is literally the first moment a market exists, which is often a 100x+ volatile day [[coinledger-blog-uniswap-airdrop-taxes-2026-04-20]].

## The phantom-income problem

Across ordinary-income-on-receipt regimes (US, AU, most EU), airdropped tokens create a well-known trap: the recipient owes tax on the FMV at a peak moment, then the token craters, leaving them with a tax bill larger than the token's final value. Partial mitigation: dispose immediately upon receipt to convert the tax into cash. No jurisdiction in the corpus offers a loss-recovery mechanism for the phantom-income case beyond ordinary capital-loss rules (which typically cannot offset ordinary income beyond small annual caps — see [[tax-loss-harvesting]]).

## Why the active/passive line matters

Germany's **passive airdrop = tax-free** rule [[coinledger-guide-germany-2026-04-20]] is the single most favorable OECD treatment. UK's similar posture [[coinledger-guide-united-kingdom-2026-04-20]] makes the distinction load-bearing — whether the user paid gas, signed a message, or did an off-chain action all matter for classification. The US flat income treatment makes the question moot domestically.

## Related wiki pages

- [[hard-fork-taxation]], [[staking-rewards]], [[defi-tax-treatment]], [[united-states]], [[germany]], [[united-kingdom]], [[australia]], [[canada]], [[spain]], [[new-zealand]], [[form-1099-misc]].

## Primary guidance

- **US:** Notice 2014-21; Rev. Rul. 2019-24 (by analogy) [primary source not yet ingested].
- **Germany:** §23 EStG; 2022 BMF letter [primary source not yet ingested].
- **UK:** HMRC Cryptoassets Manual CRYPTO21250 [primary source not yet ingested].
- **Australia:** ATO crypto airdrops guidance [primary source not yet ingested].

## Gaps

- Exact moment of "receipt" for claimed-airdrops where a user has the right but hasn't yet signed the claim transaction.
- Treatment of "sybil-filtered" airdrops where the receipt is contingent on the protocol's anti-sybil review.
- Denmark, Sweden, Ireland airdrop-specific regulator positions not in the ingested corpus.
- NFT airdrops vs fungible-token airdrops treatment variance.
