---
title: DeFi tax treatment (cross-jurisdictional)
type: concept
jurisdiction: [US, UK, DE, CA, AU, ES, SE, IE]
created: 2026-04-20
updated: 2026-04-20
tags: [defi, liquidity-pool, lending, conservative-treatment]
sources: [[coinledger-blog-defi-crypto-tax-guide-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]], [[coinledger-guide-united-kingdom-2026-04-20]], [[coinledger-guide-germany-2026-04-20]], [[coinledger-guide-canada-2026-04-20]], [[coinledger-guide-australia-2026-04-20]]
---

## Definition

"DeFi" covers non-custodial on-chain transactions: DEX swaps, liquidity provision, lending/borrowing protocols, yield farming, restaking, and synthetic/perpetual derivatives. Tax treatment varies enormously because **most jurisdictions have issued no explicit DeFi guidance** [[coinledger-blog-defi-crypto-tax-guide-2026-04-20]].

## Absence-of-guidance pattern

The IRS has **not issued explicit DeFi guidance** beyond the 2024-2025 broker regulations (which were partially repealed by Congressional Review Act resolution) [[coinledger-guide-united-states-2026-04-20]]. The HMRC Cryptoassets Manual is the **global outlier** — it has explicit DeFi sections (CRYPTO61640, CRYPTO61674) covering lending, staking, LP, and collateral [[coinledger-guide-united-kingdom-2026-04-20]]. Germany, Canada, Australia, Spain, Sweden, Ireland, Japan, and most other OECD regimes have no DeFi-specific guidance; practitioners extrapolate from general crypto rules [[coinledger-guide-germany-2026-04-20]], [[coinledger-guide-canada-2026-04-20]], [[coinledger-guide-australia-2026-04-20]].

## The conservative-treatment baseline

In the absence of guidance, CoinLedger and the practitioner consensus apply a conservative line [[coinledger-blog-defi-crypto-tax-guide-2026-04-20]]:

- **DEX swap (ETH → USDC):** Taxable crypto-to-crypto disposal. Gain/loss = proceeds (USDC FMV) − ETH basis [[coinledger-blog-defi-crypto-tax-guide-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]].
- **LP deposit (ETH + USDC → LP token):** **Taxable disposal** of both ETH and USDC; acquisition of LP token at FMV [[coinledger-guide-united-states-2026-04-20]]. Non-conservative alternative: treat as deposit, not disposal (minority practitioner view).
- **LP withdrawal (LP token → ETH + USDC):** Disposal of LP token; acquisition of underlying at FMV.
- **Lending deposit (supply USDC to Aave → aUSDC):** US conservative treatment: crypto-to-crypto disposal. UK per HMRC: "beneficial ownership" test — if you retain beneficial ownership, not a disposal (a softer line than US) [[coinledger-guide-united-kingdom-2026-04-20]].
- **Collateralized borrow (deposit ETH → receive loan USDC):** Loan receipt is not income. Collateral posting generally not a disposal if beneficial ownership retained. UK guidance explicit on this [[coinledger-guide-united-kingdom-2026-04-20]].
- **Liquidation:** Disposal of the liquidated collateral.
- **Yield (interest, farming rewards):** Ordinary income at FMV on receipt [[coinledger-blog-defi-crypto-tax-guide-2026-04-20]].
- **Wrapping (ETH ↔ WETH):** US ambiguous — conservative treats as disposal. UK HMRC treats wrapping where a different token is received as a disposal [[coinledger-guide-united-kingdom-2026-04-20]].

## Variance highlights

- **UK has the most developed DeFi doctrine.** Beneficial-ownership test for collateral deposits is taxpayer-favorable relative to US conservative baseline [[coinledger-guide-united-kingdom-2026-04-20]].
- **Germany** applies §23 EStG 12-month clock to DeFi tokens received; disposal after 12 months is tax-free, a meaningful advantage for LP positions held long-term [[coinledger-guide-germany-2026-04-20]].
- **Spain** may treat certain DeFi lending yield as interest income at the favorable 19–26% rate (same rationale as staking) [[coinledger-guide-spain-2026-04-20]].
- **Sweden** likewise routes lending yield to interest at flat 30% [[coinledger-guide-sweden-2026-04-20]].

## Why it matters

- **Lot-multiplication.** A user with 100 DEX swaps + 20 LP rebalances + daily yield receipts can generate thousands of taxable events per year. Tax software is the only feasible approach.
- **Basis-establishment cascade.** Each conservative-treatment disposal establishes new basis for the downstream asset. Missing one intermediate step propagates [[missing-cost-basis]] warnings (see [[missing-cost-basis]]).
- **Impermanent loss is unrecognized.** LP impermanent loss is not a deductible loss — it's unrealized basis decay. Realized only on LP withdrawal / disposal.
- **Broker rule retrenchment.** The 2024 DeFi broker regulations were repealed by Congressional Review Act action in 2025 [primary source not yet ingested]; DeFi protocols are **not** required to issue 1099-DA under current US rules [[coinledger-guide-united-states-2026-04-20]].

## Related wiki pages

- [[staking-rewards]], [[airdrop-taxation]], [[hard-fork-taxation]], [[nft-tax-treatment]], [[tax-loss-harvesting]], [[missing-cost-basis]], [[united-states]], [[united-kingdom]], [[germany]].

## Primary guidance

- **US:** Notice 2014-21; no DeFi-specific Rev. Ruls. in ingested corpus [primary source not yet ingested].
- **UK:** HMRC Cryptoassets Manual CRYPTO61000 DeFi sections [primary source not yet ingested].
- **DeFi broker rule:** Final reg → CRA resolution [primary source not yet ingested].

## Gaps

- US perpetuals/futures on decentralized venues (GMX, dYdX v4): no explicit guidance.
- Rebasing tokens (wrapped stETH, rebasing stablecoins) basis-tracking.
- Airdrops downstream of LP participation (protocol rewards to LPs).
- Cross-chain bridge disposal treatment — is wrapping-to-bridge a disposal?
