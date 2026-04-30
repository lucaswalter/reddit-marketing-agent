---
title: United Kingdom
type: jurisdiction
created: 2026-04-20
updated: 2026-04-20
tags: [united-kingdom, hmrc, eu-adjacent]
sources: [[coinledger-guide-united-kingdom-2026-04-20]]
---

## Classification

Cryptocurrency ("cryptoassets" per HMRC) is subject to **capital gains tax** (disposals) and **income tax** (earnings). HMRC has produced an explicit Cryptoassets Manual covering most scenarios including DeFi [[coinledger-guide-united-kingdom-2026-04-20]].

## Tax treatment by transaction type

- **Dispositions (sell, crypto-to-crypto trade, spend):** CGT on gain [[coinledger-guide-united-kingdom-2026-04-20]].
- **Compensation in crypto:** Ordinary income at FMV. Subsequent disposal triggers CGT.
- **Mining (hobby):** Miscellaneous income (declared separately on Self Assessment). £1,000/yr de minimis under which no Self Assessment needed.
- **Mining (business):** Trading profits subject to income tax. Expenses deductible.
- **Staking:** Income at FMV on receipt. HMRC Cryptoassets Manual provides explicit guidance.
- **Airdrops:** Income **only if** received in exchange for a service or action. Passive airdrops not income on receipt; CGT on disposal.
- **Hard forks:** Not specifically detailed in guide but likely similar to passive airdrop treatment.
- **NFTs:** Taxed like crypto on disposal, **but NOT subject to pooling** — each NFT is a distinct asset for basis tracking [[coinledger-guide-united-kingdom-2026-04-20]].
- **DeFi:** HMRC has explicit guidance (crypto61674 and related manual sections). Staking/LP often CGT events when different tokens are received (e.g. ETH ↔ stETH as a disposal).
- **DeFi loans:** Posting collateral generally NOT a disposal. Becomes disposal if collateral moved cross-platform or beneficial ownership transferred.
- **Gifts:** Spouse/civil-partner gifts tax-free and outside CGT allowance. Other gifts = CGT disposal at FMV.
- **Donations:** Income Tax relief. Capital gain may arise if FMV > basis, or "tainted donation" arrangement.
- **Inheritance:** Crypto counts toward estate; £325K threshold for inheritance tax.
- **VAT:** **None** on fiat↔crypto exchange. Standard VAT on crypto-paid goods/services.
- **Worthless / lost keys:** Negligible value claim — treat as disposed at £0 to crystallize loss.
- **Tax-free:** Holding, wallet-to-wallet transfers, spouse gifts.

## Rates and thresholds

- **CGT rates (post Oct 30, 2024 Autumn Budget):** 18% (basic rate band) / 24% (higher and additional rate bands). Up from 10/20% pre-budget [[coinledger-guide-united-kingdom-2026-04-20]].
- **Annual CGT exemption:** **£3,000** (2024-25), down from £6,000 (2023-24) and £12,600 historically. Sharply tightened.
- **Income tax:** 0% personal allowance up to £12,570 / 20% / 40% / 45%. Personal allowance withdrawn above £125,140. (Scotland has different rates.)
- **Inheritance tax threshold:** £325K.
- **Mining hobby de minimis:** £1,000.

## Cost basis method

- **Shared Pool Accounting (Section 104 pool)** — an average-cost method where each cryptocurrency has its own pool [[coinledger-guide-united-kingdom-2026-04-20]].
- **Matching order (anti-wash-sale):**
  1. **Same Day Rule:** Same-day buys matched to same-day sales first.
  2. **Bed & Breakfast Rule (30 days):** Coins bought within 30 days after a sale match to that sale before entering the pool.
  3. **Section 104 pool:** Remainder uses average-cost.
- **NFTs are exempt from pooling** — each treated as a distinct asset.

## Reporting forms and deadlines

- **Tax year:** April 6 – April 5 [[coinledger-guide-united-kingdom-2026-04-20]].
- **Paper Self Assessment deadline:** October 31.
- **Online Self Assessment deadline:** January 31.
- Self Assessment tax return with CGT pages.
- Capital losses must be **registered within 4 years** of the tax year or are lost.

## Losses

- Capital losses offset capital gains in-year [[coinledger-guide-united-kingdom-2026-04-20]].
- Carry forward **indefinitely** once registered.
- **Must register within 4 years** to use later — unusual and easy to miss.
- Same Day + B&B rules prevent wash-sale harvesting.
- Negligible value claims for worthless tokens or lost keys.

## Regulator and primary guidance

- Primary regulator: [[hmrc]] (His Majesty's Revenue and Customs).
- Key guidance: HMRC Cryptoassets Manual (CRYPTO10000 onward, with sections including CRYPTO20250 on business vs hobby trading and CRYPTO61640, CRYPTO61674 on DeFi).

## Notable quirks

- **Shared Pool Accounting** — HMRC's version of average-cost — unique pooling treatment vs FIFO-default regimes [[coinledger-guide-united-kingdom-2026-04-20]].
- **Same Day + Bed & Breakfast (30-day) matching** — explicit anti-wash-sale rules applying to crypto [[coinledger-guide-united-kingdom-2026-04-20]].
- **NFTs exempt from pooling** — unlike UK stocks-and-shares treatment [[coinledger-guide-united-kingdom-2026-04-20]].
- **Autumn Budget 2024 mid-year CGT rate change** (18/24% effective Oct 30, 2024) creates dual-rate year [[coinledger-guide-united-kingdom-2026-04-20]].
- **Annual exemption collapsed from £12,600 → £3,000** over 2 years — more crypto traders now in scope.
- **HMRC Cryptoassets Manual is one of the most detailed regulator publications globally**, including explicit DeFi guidance that few other tax authorities have produced.
- **Coinbase automatic data share** with HMRC at £5K fiat-inflow threshold per Coinbase email to customers.

## Enforcement

- HMRC has data-sharing agreements with Coinbase and other major exchanges [[coinledger-guide-united-kingdom-2026-04-20]].
- Nudge letters sent to investors.
- Penalty: 20% CGT + interest + up to 200% penalty for evasion. Criminal charges possible.
- Amended Self Assessment allows reporting prior-year omissions.

## Record retention

- Standard 5-year rule for Self Assessment taxpayers (not explicitly in source but UK norm).

## Gaps

- Latest CGT allowance value (£3,000 confirmed for 2024-25; 2025-26 not stated).
- Explicit hard-fork guidance.
- Stablecoin-specific treatment.
- Collectibles-style NFT treatment.
- Treatment of margin/futures/perpetuals.
- Scotland-specific income tax rates.
- Interaction with Crypto-Asset Reporting Framework (CARF) / EU DAC8 (UK post-Brexit).
