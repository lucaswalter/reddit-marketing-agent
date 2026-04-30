---
title: NFT tax treatment (cross-jurisdictional)
type: concept
jurisdiction: [US, UK, CA, AU, DE, IE]
created: 2026-04-20
updated: 2026-04-20
tags: [nft, collectibles, creator, collector]
sources: [[coinledger-blog-how-are-nfts-taxed-2026-04-20]], [[coinledger-blog-nft-tax-australia-2026-04-20]], [[coinledger-blog-nft-tax-canada-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]], [[coinledger-guide-united-kingdom-2026-04-20]], [[coinledger-guide-australia-2026-04-20]], [[coinledger-guide-canada-2026-04-20]], [[coinledger-guide-germany-2026-04-20]]
---

## Definition

A non-fungible token (NFT) is a unique digital asset verified on a blockchain — typically ERC-721 or ERC-1155 on Ethereum or equivalent on other chains [[coinledger-blog-how-are-nfts-taxed-2026-04-20]]. Tax treatment diverges along two axes: **creator vs collector** and **collectibles vs generic-crypto** classification.

## US: the collectibles question

The IRS has flagged in **Notice 2023-27** that some NFTs may constitute **collectibles** under IRC §408(m)(2), subject to the **28% maximum long-term capital gains rate** instead of the usual 20% top rate [primary source not yet ingested], [[coinledger-guide-united-states-2026-04-20]]. The "look-through" analysis: if the NFT represents a digital work of art, a gem, a stamp, or other §408(m)(2) property, it's a collectible.

Practical implications [[coinledger-blog-how-are-nfts-taxed-2026-04-20]]:
- **Profile-pic / art NFTs (Bored Ape, CryptoPunks):** Likely collectibles → 28% LTCG rate cap.
- **Utility NFTs (membership passes, gaming items):** Likely not collectibles → standard 20% LTCG cap.
- **Fractional NFTs, NFT ETFs:** Partially-determinable — look-through applies to the underlying.

No ingested source has a safe-harbor list; classification is facts-and-circumstances.

## Variance across jurisdictions

| Jurisdiction | Collector (buying/selling) | Creator (minting/selling) | Special features |
|---|---|---|---|
| **US** | Capital gain/loss; 28% LTCG if collectible | Ordinary income on primary sale | [[coinledger-guide-united-states-2026-04-20]] |
| **UK** | CGT on disposal; **NFTs exempt from Section 104 pooling** — each NFT a distinct asset | Income on sale | [[coinledger-guide-united-kingdom-2026-04-20]] |
| **Canada** | CGT on disposal; 50% inclusion | Business income | [[coinledger-blog-nft-tax-canada-2026-04-20]], [[coinledger-guide-canada-2026-04-20]] |
| **Australia** | CGT; 50% discount if >12mo | Ordinary income on mint/primary sale | [[coinledger-blog-nft-tax-australia-2026-04-20]], [[coinledger-guide-australia-2026-04-20]] |
| **Germany** | §23 EStG 12-month rule by analogy; tax-free if >12mo hold | Ordinary income on creator sale | [[coinledger-guide-germany-2026-04-20]] |
| **Ireland** | CGT; buying NFT with crypto = crypto disposal (double-event) | Income on primary/secondary sales | [[coinledger-guide-ireland-2026-04-20]] |
| **New Zealand** | Income; GST on NZ-domestic buyer sales | Income + GST on NZ sales; no GST on foreign buyers | [[coinledger-guide-new-zealand-2026-04-20]] |

## The UK pooling exemption

HMRC treats NFTs as distinct assets — **exempt from Section 104 shared-pool accounting** that applies to fungible cryptoassets (see [[shared-pool-accounting]]) [[coinledger-guide-united-kingdom-2026-04-20]]. Each NFT is tracked individually with its own acquisition-date and cost basis. This mirrors HMRC's treatment of shares in different companies (not pooled) vs. shares in the same company (pooled).

## The double-disposal on NFT purchase

Buying an NFT with ETH (or any crypto) is a **disposal of the ETH** and an **acquisition of the NFT** [[coinledger-blog-how-are-nfts-taxed-2026-04-20]], [[coinledger-guide-ireland-2026-04-20]]. This is consistent across jurisdictions and is the #1 NFT tax-compliance miss in practice — the user recognizes an NFT price but not the embedded crypto-to-crypto gain on the ETH used to pay.

## Creator treatment

Primary-sale proceeds are **ordinary income** in every ingested jurisdiction [[coinledger-blog-how-are-nfts-taxed-2026-04-20]], [[coinledger-blog-nft-tax-australia-2026-04-20]]. Royalties from secondary sales are typically royalty income (Schedule E in US, or Schedule C if a creator business). NFT mint costs (gas, platform fees) generally deductible against creator income but not against collector capital gains (the Tax Cuts and Jobs Act disallowed miscellaneous investment expenses through 2025 in the US) [uncited].

## Related wiki pages

- [[defi-tax-treatment]], [[shared-pool-accounting]], [[missing-cost-basis]], [[tax-loss-harvesting]], [[united-states]], [[united-kingdom]], [[germany]], [[canada]], [[australia]], [[ireland]].

## Primary guidance

- **US:** Notice 2023-27 (NFT collectibles treatment); IRC §408(m)(2) [primary source not yet ingested].
- **UK:** HMRC Cryptoassets Manual CRYPTO40000-series (NFT sections) [primary source not yet ingested].

## Gaps

- Collectibles look-through methodology: no bright-line IRS guidance.
- NFT-as-loan-collateral tax treatment.
- Play-to-earn in-game NFT receipt (Axie-style) — income vs. receipt/disposal split.
- Royalty-enforcement moves (OpenSea 0% royalty shift) and creator tax character if royalties become optional.
- Fractionalized NFTs (F-NFTs) and ERC-404 hybrids.
