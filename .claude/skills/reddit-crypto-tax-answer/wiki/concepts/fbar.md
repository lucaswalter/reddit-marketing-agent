---
title: FBAR (FinCEN Form 114 — Report of Foreign Bank and Financial Accounts)
type: concept
jurisdiction: [US]
created: 2026-04-20
updated: 2026-04-20
tags: [us, fincen, foreign-accounts, reporting]
sources: [[coinledger-blog-fbar-reporting-requirements-for-cryptocurrency-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]]
---

## Definition

FinCEN Form 114 — the "FBAR" — is a Treasury/FinCEN (not IRS) annual report filed by US persons with **financial interest in or signature authority over foreign financial accounts** whose aggregate highest daily balance exceeded **$10,000** at any point during the calendar year [primary source not yet ingested — 31 USC §5314, 31 CFR §1010.350]. Filed separately from the income tax return, due April 15 with an automatic extension to October 15.

## The open crypto question

FinCEN has **not yet required** FBAR reporting for cryptocurrency held at foreign exchanges [[coinledger-blog-fbar-reporting-requirements-for-cryptocurrency-2026-04-20]]. The governing 2020 event: FinCEN issued **Notice 2020-2** stating foreign virtual-currency accounts were not (yet) FBAR-reportable and simultaneously announced a Notice of Proposed Rulemaking (NPRM) that would extend FBAR to virtual-currency accounts [primary source not yet ingested].

The NPRM has **never been finalized**. Subsequent FinCEN silence — no further notice, no regulatory action — leaves the 2020 Notice as the operative position through the ingested corpus date. The conservative-practice position is to file anyway if aggregate holdings at foreign exchanges exceed $10K [[coinledger-blog-fbar-reporting-requirements-for-cryptocurrency-2026-04-20]].

## Scope questions still live

- **Foreign exchanges.** [[coinbase]] is US-based; Binance.com, KuCoin, Bitfinex, OKX are non-US. Holdings at these platforms are the archetypal FBAR-candidate case [[coinledger-blog-fbar-reporting-requirements-for-cryptocurrency-2026-04-20]].
- **Self-custody.** A hardware wallet holding crypto is almost certainly not a "foreign account" under any reasonable reading — it has no custodian and no foreign location in the §1010.350 sense [uncited].
- **Non-custodial DeFi.** A smart contract deposit (Aave, Compound) doesn't fit a "foreign financial account" concept cleanly; there is no custodian and no jurisdiction.
- **Hybrid custody.** Exchange sub-accounts, prime-brokerage structures, and wrapped-asset bridges complicate the mapping.

## Practical penalty exposure

FBAR non-willful penalty: up to **$10,000 per violation** (per account, per year). Willful: greater of $100,000 or 50% of account balance [primary source not yet ingested]. The conservative position — file when in doubt — is driven by the severity of willful-penalty exposure against the practically-zero downside of filing when not required.

## Status of Form 8938 (FATCA)

Distinct from FBAR: Form 8938 reports Specified Foreign Financial Assets above thresholds ($50K/$100K single / $100K/$150K MFJ) and is filed **with** the 1040. IRS has similarly not explicitly confirmed crypto inclusion [primary source not yet ingested]. The CoinLedger US guide treats this as an open question [[coinledger-guide-united-states-2026-04-20]].

## Related wiki pages

- [[united-states]], [[irs]], [[cp2000]], [[carf]], [[dac8]].

## Primary guidance

- 31 USC §5314; 31 CFR §1010.350 [primary source not yet ingested].
- FinCEN Notice 2020-2 [primary source not yet ingested].
- FinCEN 2020 NPRM (digital asset FBAR extension — never finalized) [primary source not yet ingested].

## Gaps

- Current FinCEN status of the NPRM through 2025–2026 — no ingested source post-dates the 2020 NPRM.
- Interaction with CARF-era CASP reporting (see [[carf]]) — whether multilateral information-sharing eventually makes FBAR redundant.
- Form 8938 crypto-reporting requirements and thresholds.
- Treatment of foreign-exchange-hosted staking and earn products under the "account" concept.
