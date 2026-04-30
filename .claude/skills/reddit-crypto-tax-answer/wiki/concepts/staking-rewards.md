---
title: Staking rewards (tax treatment)
type: concept
jurisdiction: [US, UK, DE, CA, AU, ES, SE, NZ]
created: 2026-04-20
updated: 2026-04-20
tags: [staking, ordinary-income, dominion-and-control, cross-jurisdictional]
sources: [[coinledger-blog-staking-taxes-2026-04-20]], [[coinledger-blog-cardano-staking-tax-2026-04-20]], [[coinledger-blog-solana-staking-taxes-2026-04-20]], [[coinledger-blog-bnb-staking-tax-2026-04-20]], [[coinledger-blog-how-is-tron-staking-taxed-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]], [[coinledger-guide-united-kingdom-2026-04-20]], [[coinledger-guide-germany-2026-04-20]], [[coinledger-guide-canada-2026-04-20]], [[coinledger-guide-australia-2026-04-20]], [[coinledger-guide-spain-2026-04-20]], [[coinledger-guide-sweden-2026-04-20]], [[coinledger-guide-new-zealand-2026-04-20]]
---

## Definition

Staking rewards are tokens received for participating in a Proof-of-Stake consensus mechanism (validator or delegator) or analogous on-chain mechanism (liquid-staking derivatives, app-level staking). Across jurisdictions the **universal default** is ordinary income at FMV on receipt, but the receipt-timing rule and the income-character classification vary [[coinledger-blog-staking-taxes-2026-04-20]].

## US: Rev. Rul. 2023-14 and dominion-and-control

IRS position, codified in **Rev. Rul. 2023-14** [primary source not yet ingested]: staking rewards are ordinary income at FMV **when the taxpayer gains dominion and control** — i.e., when rewards can be sold, exchanged, or otherwise disposed of [[coinledger-blog-staking-taxes-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]]. Reported on Schedule 1, Line 8 via [[form-1099-misc]] if issued; otherwise self-reported. Subsequent disposal: capital gain/loss on [[form-8949]] [[coinledger-blog-staking-taxes-2026-04-20]].

Dominion-and-control timing matters for protocols with delayed reward release:
- **Ethereum post-Shanghai:** Rewards accrue in the beacon layer; withdrawable since April 2023. Receipt likely at each distribution; some practitioners use a continuous-accrual approach [uncited].
- **Cardano:** Rewards auto-compound but are immediately available — receipt at each epoch distribution [[coinledger-blog-cardano-staking-tax-2026-04-20]].
- **Solana:** Auto-delegated rewards; dominion at each epoch [[coinledger-blog-solana-staking-taxes-2026-04-20]].
- **Locked/bonded staking** (Cosmos 21-day unbonding, etc.): dominion contested — unlockable balance is receivable but not transferable.

The pre-2023 *Jarrett v. United States* case — where a taxpayer argued staking rewards are not income until sold (analogous to baked bread / extracted gold) — was dismissed; Rev. Rul. 2023-14 effectively closed the argument [primary source not yet ingested].

## Variance across jurisdictions

| Jurisdiction | Treatment | Rate character |
|---|---|---|
| **US** | Ordinary income on receipt (dominion-and-control); CGT on disposal | Marginal ordinary rate [[coinledger-guide-united-states-2026-04-20]] |
| **UK** | Miscellaneous income on receipt; CGT on disposal (HMRC explicit) | Income tax rate on receipt portion [[coinledger-guide-united-kingdom-2026-04-20]] |
| **Germany** | Ordinary income on receipt; disposal tax-free if held >12mo (§23 EStG) [[coinledger-guide-germany-2026-04-20]] | Ordinary rate; zero on long-term disposal |
| **Canada (individual)** | Income at FMV on receipt; CGT on disposal [[coinledger-guide-canada-2026-04-20]] | Ordinary / 50% inclusion on disposal |
| **Canada (business)** | Business income on receipt + disposal | 100% inclusion |
| **Australia** | Ordinary income at FMV on receipt [[coinledger-guide-australia-2026-04-20]] | Marginal ordinary rate |
| **Spain** | **Interest income** at 19–26% (favorable treatment) [[coinledger-guide-spain-2026-04-20]] | Savings-income rate |
| **Sweden** | **Interest income** at 30% flat (staking ≈ lending crypto to network) [[coinledger-guide-sweden-2026-04-20]] | Flat 30% |
| **New Zealand** | Ordinary income at FMV on receipt; income/loss on disposal delta [[coinledger-guide-new-zealand-2026-04-20]] | Marginal ordinary |

## The Spain/Sweden interest-income variance

The genuine policy split: **Spain and Sweden treat staking as interest income** [[coinledger-guide-spain-2026-04-20]], [[coinledger-guide-sweden-2026-04-20]]. The rationale is that staking functionally resembles lending crypto to the network in exchange for yield. This gives favorable rates (savings-income tiers) compared to treating staking as mining-style ordinary income. The majority of ingested jurisdictions reject this framing.

## Liquid staking

No ingested jurisdiction has explicit guidance on **liquid staking derivatives** (stETH, rETH, JitoSOL). The US conservative position: the ETH→stETH conversion may itself be a disposal (crypto-to-crypto trade); subsequent rebasing or reward accrual is income at dominion-and-control. The UK HMRC Cryptoassets Manual explicitly treats ETH↔stETH as a CGT disposal when different tokens are received [[coinledger-guide-united-kingdom-2026-04-20]].

## Related wiki pages

- [[airdrop-taxation]], [[hard-fork-taxation]], [[defi-tax-treatment]], [[form-1099-misc]], [[form-8949]], [[united-states]], [[united-kingdom]], [[germany]], [[canada]], [[australia]], [[spain]], [[sweden]], [[new-zealand]].

## Primary guidance

- **US:** Rev. Rul. 2023-14; Notice 2014-21 [primary source not yet ingested].
- **UK:** HMRC Cryptoassets Manual (staking sections) [primary source not yet ingested].
- **Germany:** §23 EStG; 2022 BMF letter [primary source not yet ingested].

## Gaps

- MEV rewards, restaking (EigenLayer), and validator-tip income: no explicit jurisdictional guidance in corpus.
- Pooled-staking tax lot attribution (Lido rebasing token vs. wrapped) — open.
- Denmark/Ireland/Japan staking specifics not deeply covered.
