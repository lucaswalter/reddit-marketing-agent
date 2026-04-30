---
title: Shared Pool Accounting (UK Section 104)
type: concept
jurisdiction: [UK]
created: 2026-04-20
updated: 2026-04-20
tags: [uk, hmrc, section-104, cost-basis, pooling]
sources: [[coinledger-guide-united-kingdom-2026-04-20]]
---

## Definition

The UK's mandated cost-basis method for fungible cryptoassets: each cryptocurrency has its own **Section 104 pool** containing all the taxpayer's units of that asset at a running **average cost** [[coinledger-guide-united-kingdom-2026-04-20]]. On disposal, the cost basis used is the pool's average — not a specific lot. Acquisitions and disposals adjust the pool's total units and total pool cost.

Section 104 is a provision of the **Taxation of Chargeable Gains Act 1992** (TCGA 1992 s.104) [primary source not yet ingested], originally written for shares and applied to cryptoassets via HMRC Cryptoassets Manual.

## Mechanics

**Pool = (Σ acquisition cost) / (Σ units held).** Each buy adds units and cost; each sell removes units and a proportional share of cost.

Worked example: buy 1 BTC at £20K, later buy 1 BTC at £40K. Pool: 2 BTC at £60K total → £30K/BTC average. Sell 1 BTC at £50K → proceeds £50K, cost basis £30K, gain £20K. Pool now holds 1 BTC at £30K.

## Matching order (the anti-wash-sale overlay)

On disposal, HMRC applies a specific matching order **before** touching the Section 104 pool [[coinledger-guide-united-kingdom-2026-04-20]]:

1. **Same Day Rule** — disposals match same-day acquisitions of the same asset first.
2. **Bed & Breakfast Rule (30-day)** — next, match against acquisitions of the same asset within 30 days **after** the disposal (see [[bed-and-breakfast-rule]]).
3. **Section 104 pool** — the remainder uses the pool's average cost.

The matching order prevents wash-sale-style loss harvesting. A user who sells at a loss and rebuys the same asset within 30 days will have the loss neutralized — the disposal matches against the reacquired lot at its actual cost rather than the pool's average, typically eliminating or dramatically reducing the realized loss [[coinledger-guide-united-kingdom-2026-04-20]].

## NFT exemption

**NFTs are not subject to Section 104 pooling** [[coinledger-guide-united-kingdom-2026-04-20]]. Each NFT is a distinct asset tracked independently, mirroring the HMRC treatment of shares in different companies (pooled only within the same company). See [[nft-tax-treatment]].

## Why it matters

- **No Spec-ID.** A UK taxpayer cannot elect HIFO or LIFO to minimize gain; the Section 104 average is the only available basis [[coinledger-guide-united-kingdom-2026-04-20]].
- **Tax-loss harvesting is structurally constrained.** Combined with Same Day + 30-day B&B, the UK matching regime blocks the US-style TLH tactic of sell-and-rebuy-same-day (see [[tax-loss-harvesting]], [[wash-sale-rule]]).
- **Cross-software reconciliation.** A UK user migrating between tax platforms needs consistent pool state — a mid-year handoff without the pool's full acquisition history produces wrong outputs.
- **Stablecoins are pooled the same way.** Every USDC buy/sell cycles through the USDC pool. Disposals generate near-zero gain (stablecoin price ≈ pool average ≈ 1 GBP equivalent) but are still reportable events.
- **Mixed-acquisition-context pool.** The pool doesn't distinguish between coins acquired via purchase, staking reward, or airdrop — once in the pool, character is lost. HMRC guidance on this is that the pool captures both capital (purchase) and income-derived (staking reward at FMV) basis (see [[staking-rewards]]).

## Product implication (CoinLedger)

Section 104 accounting is materially different from the US/AU per-lot FIFO/HIFO engines. Any crypto-tax platform serving UK users needs dedicated pool-mutation logic and matching-order sequencing. The jurisdiction page notes this as load-bearing [[coinledger-guide-united-kingdom-2026-04-20]].

## Related wiki pages

- [[bed-and-breakfast-rule]], [[cost-basis-methods]], [[wash-sale-rule]], [[tax-loss-harvesting]], [[nft-tax-treatment]], [[united-kingdom]], [[hmrc]].

## Primary guidance

- TCGA 1992 s.104 [primary source not yet ingested].
- HMRC Cryptoassets Manual CRYPTO22150–22250 (pooling sections) [primary source not yet ingested].

## Gaps

- Cross-wallet pool behavior — the UK pool is notionally taxpayer-level, not wallet-level, but exchange 1099-DA-equivalent reporting is a UK unknown.
- Treatment of wrapped tokens (WBTC vs BTC, stETH vs ETH) — same pool or separate?
- Pool state at emigration (UK→non-UK tax residence change).
