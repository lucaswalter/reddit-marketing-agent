---
title: Form 1099-B (Proceeds From Broker and Barter Exchange Transactions)
type: concept
jurisdiction: [US]
created: 2026-04-20
updated: 2026-04-20
tags: [us, irs, 1099, broker-reporting]
sources: [[coinledger-blog-form-1099-b-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]], [[coinledger-blog-crypto-form-1099-2026-04-20]]
---

## Definition

Legacy US [[irs]] information return filed by brokers to report customer proceeds from securities sales, covered-security cost basis, and capital-gain/loss character. Pre-digital-asset era, 1099-B was the canonical reporting instrument for brokerage sales [[coinledger-blog-form-1099-b-2026-04-20]].

## Crypto's historical relationship

Most crypto exchanges did **not** issue 1099-B to customers [[coinledger-blog-form-1099-b-2026-04-20]]. The form was built around "broker" as defined for securities reporting, and pre-2024 the definition didn't cleanly reach crypto exchanges. A minority of exchanges (Robinhood Crypto for a period; some US-regulated platforms) did issue 1099-B for crypto trades — creating practitioner confusion when a user's records included a 1099-B from one venue and nothing from the rest of their footprint.

Where a crypto 1099-B was issued, it often had the same cost-basis accuracy problem that now plagues [[form-1099-da]]: proceeds correct, basis missing or wrong whenever crypto had been transferred in from elsewhere [[coinledger-blog-form-1099-b-2026-04-20]].

## Transition to 1099-DA

Starting in tax year 2025, digital-asset broker reporting shifts to the dedicated **Form 1099-DA** under the Infrastructure Investment and Jobs Act broker rules [[coinledger-guide-united-states-2026-04-20]]. All US-operating exchanges are required to report capital gains and losses to the IRS [[coinledger-blog-form-1099-b-2026-04-20]]. 1099-DA supersedes 1099-B for crypto; exchanges that previously issued 1099-B for crypto will migrate. See [[form-1099-da]] for the successor regime.

## Why the transition matters

- **Taxpayer burden shifts.** Pre-1099-DA, the IRS had proceeds data via John Doe summonses and 1099-K (see [[form-1099-k]]) but not structured per-lot reporting. Post-transition, every disposal is on record.
- **Reconciliation becomes the support job.** Crypto tax software no longer just computes 8949s from trade data; it reconciles against the 1099-DA the IRS also received [[coinledger-blog-form-1099-b-2026-04-20]].
- **Basis tracking enforcement.** 1099-B's "covered security" concept (broker tracks basis) informs the 1099-DA phased basis-reporting schedule — exchanges aren't required to track basis for 2025 but are expected to in later phases [[coinledger-blog-form-1099-b-2026-04-20]].

## Related wiki pages

- [[form-1099-da]], [[form-1099-k]], [[form-1099-misc]], [[form-8949]], [[united-states]], [[irs]], [[cp2000]].

## Primary guidance

- IRC §6045 (broker information returns) [primary source not yet ingested].
- Infrastructure Investment and Jobs Act broker provisions (2021) [primary source not yet ingested].
- Final broker regulations TD 10000 (2024) [primary source not yet ingested].

## Gaps

- Which crypto brokerages issued 1099-B pre-2025 and on what schedule — no ingested source has this list.
- Whether 1099-B issued by a broker that also files 1099-DA for the same period produces double-reporting (the IRS guidance anticipates this but mechanics are not in the ingested corpus).
