---
title: Form 1099-K (Payment Card and Third Party Network Transactions)
type: concept
jurisdiction: [US]
created: 2026-04-20
updated: 2026-04-20
tags: [us, irs, 1099, payment-processor, cp2000]
sources: [[coinledger-blog-what-to-do-with-your-1099-k-from-coinbase-gemini-or-gdax-for-crypto-taxes-2026-04-20]], [[coinledger-blog-coinbase-to-stop-reporting-form-1099-k-to-irs-2026-04-20]], [[coinledger-blog-crypto-form-1099-2026-04-20]]
---

## Definition

US [[irs]] information return originally designed for payment-card processors and third-party settlement organizations (TPSOs) to report aggregate gross proceeds credited to a payee's account. Reports **gross receipts** — not net — and contains no cost basis [[coinledger-blog-what-to-do-with-your-1099-k-from-coinbase-gemini-or-gdax-for-crypto-taxes-2026-04-20]].

## The Coinbase 1099-K era (2017–2020)

Several major US crypto exchanges — including [[coinbase]], Gemini, and GDAX — issued 1099-K to customers meeting the then-applicable thresholds (generally 200 transactions + $20,000 gross) [[coinledger-blog-what-to-do-with-your-1099-k-from-coinbase-gemini-or-gdax-for-crypto-taxes-2026-04-20]]. Coinbase discontinued 1099-K issuance after 2020 and switched reporting approaches [[coinledger-blog-coinbase-to-stop-reporting-form-1099-k-to-irs-2026-04-20]].

The fundamental problem: 1099-K reports **gross proceeds** aggregated across all dispositions in a year. For a crypto investor with high-frequency trading activity, the gross proceeds number was often an order of magnitude larger than actual taxable gain — a taxpayer who bought $10K of BTC, traded it in and out of altcoins 500 times, and ended the year with $11K would see a 1099-K with $200K+ in reported proceeds [[coinledger-blog-what-to-do-with-your-1099-k-from-coinbase-gemini-or-gdax-for-crypto-taxes-2026-04-20]].

## The CP2000 cascade

The IRS Automated Underreporter system compared 1099-K proceeds against amounts reported on returns. Discrepancies triggered **CP2000 notices** (see [[cp2000]]) proposing additional tax on the full 1099-K amount as if it were pure income [[coinledger-blog-crypto-form-1099-2026-04-20]]. This caused a well-documented wave of erroneous CP2000s to crypto traders in the 2018–2020 audit seasons — the single largest driver of crypto tax-enforcement confusion pre-1099-DA [[coinledger-blog-what-to-do-with-your-1099-k-from-coinbase-gemini-or-gdax-for-crypto-taxes-2026-04-20]].

Practitioner response: file Form 8949 with actual per-lot gain/loss, attach a reconciliation explaining that 1099-K reflects gross proceeds not income, and dispute the CP2000 with records [[coinledger-blog-what-to-do-with-your-1099-k-from-coinbase-gemini-or-gdax-for-crypto-taxes-2026-04-20]].

## The $600 threshold saga

The American Rescue Plan Act (2021) lowered the TPSO 1099-K threshold from $20,000/200 transactions to **$600** for payments received after 2021 [primary source not yet ingested]. The IRS delayed enforcement in 2023 and 2024 phased-in implementation. For crypto this was largely moot once 1099-DA was finalized, but the $600 threshold saga remains a live issue for payment apps generally.

## Status today

Post-2020 Coinbase issues **1099-MISC** for qualifying rewards/income events (see [[form-1099-misc]]) and, starting tax year 2025, [[form-1099-da]] for dispositions [[coinledger-blog-coinbase-to-stop-reporting-form-1099-k-to-irs-2026-04-20]]. 1099-K for crypto is effectively extinct at major US exchanges as of the ingested corpus.

## Related wiki pages

- [[form-1099-da]], [[form-1099-misc]], [[form-1099-b]], [[cp2000]], [[form-8949]], [[united-states]], [[irs]].

## Primary guidance

- IRC §6050W (third-party network transactions) [primary source not yet ingested].
- American Rescue Plan Act §9674 [primary source not yet ingested].
- Notice 2023-10, Notice 2023-74 (threshold delays) [primary source not yet ingested].

## Gaps

- Exact CP2000 volume attributable to crypto 1099-K mismatches — no source has hard numbers.
- Whether any crypto platform still issues 1099-K post-2024 for legacy-merchant flows.
