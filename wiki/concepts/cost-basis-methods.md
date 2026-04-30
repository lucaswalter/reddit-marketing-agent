---
title: Cost basis methods (cross-jurisdictional)
type: concept
jurisdiction: [global]
created: 2026-04-20
updated: 2026-04-20
tags: [cost-basis, fifo, lifo, hifo, acb, shared-pool, spec-id]
sources: [[coinledger-blog-cryptocurrency-tax-calculations-fifo-and-lifo-costing-methods-explained-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]], [[coinledger-guide-united-kingdom-2026-04-20]], [[coinledger-guide-canada-2026-04-20]], [[coinledger-guide-germany-2026-04-20]], [[coinledger-guide-australia-2026-04-20]], [[coinledger-guide-sweden-2026-04-20]], [[coinledger-guide-new-zealand-2026-04-20]], [[coinledger-guide-ireland-2026-04-20]], [[coinledger-guide-spain-2026-04-20]], [[coinledger-guide-south-africa-2026-04-20]], [[coinledger-guide-denmark-2026-04-20]]
---

## Definition

The method used to determine which acquired lot matches a disposal when computing capital gain/loss. For fungible assets acquired at different times and prices, the choice affects the gain/loss number materially — often 10-30% of total liability [[coinledger-blog-cryptocurrency-tax-calculations-fifo-and-lifo-costing-methods-explained-2026-04-20]].

## The canonical variants

- **FIFO (First In, First Out)** — oldest lot first. Default in most jurisdictions; typically maximizes long-term-hold qualification.
- **LIFO (Last In, First Out)** — newest lot first. Minimizes gain in a rising market (high basis first).
- **HIFO (Highest In, First Out)** — highest-basis lot first. Minimizes gain regardless of order.
- **Specific Identification (Spec-ID)** — taxpayer nominates the lot. Requires contemporaneous documentation (see [[spec-id]]).
- **Average Cost / ACB (Adjusted Cost Base)** — basis = running average across the identical-asset pool (see [[adjusted-cost-base]]).
- **Shared Pool (Section 104 pool)** — UK's average-cost variant with specific matching-order rules (see [[shared-pool-accounting]]).
- **Weighted Average Cost (WAC)** — similar to ACB; time-weighted variant.

## Cross-jurisdiction permissibility

| Jurisdiction | Default | Permitted alternatives | Notes |
|---|---|---|---|
| **US** | FIFO | Spec-ID (HIFO/LIFO via Spec-ID election) [[coinledger-guide-united-states-2026-04-20]] | Per-wallet required 2025+ (see [[per-wallet-cost-basis]]) |
| **UK** | Shared Pool (Section 104) — only method | None; mandatory [[coinledger-guide-united-kingdom-2026-04-20]] | Same Day + 30-day B&B matching precede pool (see [[shared-pool-accounting]]) |
| **Canada** | ACB — only method | None; mandatory [[coinledger-guide-canada-2026-04-20]] | Superficial Loss Rule applies (see [[superficial-loss-rule]]) |
| **Germany** | FIFO (preferred) [[coinledger-guide-germany-2026-04-20]] | Effectively FIFO only; acquisition-date tracking critical for §23 12-month rule |
| **Australia (investor)** | FIFO, LIFO, or HIFO via individual identification [[coinledger-guide-australia-2026-04-20]] | All allowed if units identifiable |
| **Australia (trader)** | FIFO only [[coinledger-guide-australia-2026-04-20]] | |
| **Ireland** | FIFO + 4-week exception [[coinledger-guide-ireland-2026-04-20]] | Most-recent-lot matching on disposals within 4 weeks of acquisition |
| **Spain** | FIFO | None [[coinledger-guide-spain-2026-04-20]] |
| **Sweden** | ACB — mandatory [[coinledger-guide-sweden-2026-04-20]] | Unusually strict; per identical-crypto pool |
| **New Zealand** | FIFO or WAC [[coinledger-guide-new-zealand-2026-04-20]] | Consistency across years recommended; no HIFO/LIFO |
| **South Africa** | FIFO or Spec-ID (inferred from stock guidance) [[coinledger-guide-south-africa-2026-04-20]] | Explicit crypto rule absent |
| **Denmark** | FIFO [[coinledger-guide-denmark-2026-04-20]] | Unknown basis → $0 (maximum taxable proceeds) |
| **Japan** | Moving Average or Total Average [primary source not yet ingested] — cited in jurisdiction page |

## The practitioner hierarchy

Rate of deviation from FIFO in crypto-tax software is roughly:
1. **US:** HIFO-via-Spec-ID is the most-elected method for gain minimization [[coinledger-blog-cryptocurrency-tax-calculations-fifo-and-lifo-costing-methods-explained-2026-04-20]].
2. **AU:** HIFO for investors, FIFO locked for traders.
3. **Jurisdictions with forced averaging** (CA, UK, SE, DE-effectively): no software-level choice.

## Why it matters

- **Rate arbitrage.** In the US, HIFO minimizes short-term gain at the cost of tranching off long-term lots. For a position with mixed holding periods, method choice interacts with STCG/LTCG rate delta.
- **1099-DA broker default.** US brokers reporting on [[form-1099-da]] generally default to FIFO unless the customer has instructed Spec-ID per-lot. Method mismatch between taxpayer software and broker report generates [[cp2000]] risk.
- **Per-wallet transition (US, 2025+).** The Rev. Proc. 2024-28 transition requires per-wallet accounting; pre-2025 universal cost basis is deprecated (see [[per-wallet-cost-basis]]).
- **UK pooling moves basis independently.** A user consistent across years must understand that Section 104 updates the pool every time they buy more of the same asset; they cannot "choose" a lot.

## Related wiki pages

- [[spec-id]], [[per-wallet-cost-basis]], [[adjusted-cost-base]], [[shared-pool-accounting]], [[superficial-loss-rule]], [[bed-and-breakfast-rule]], [[missing-cost-basis]], [[form-8949]], [[form-1099-da]].

## Primary guidance

- **US:** Treas. Reg. §1.1012-1(j); Rev. Proc. 2024-28 [primary source not yet ingested].
- **UK:** TCGA 1992 s.104 [primary source not yet ingested].
- **Canada:** ITA s.47 [primary source not yet ingested].

## Gaps

- Japan Moving Average vs Total Average mechanics not deeply covered in ingested corpus.
- UAE, India, some APAC-EU jurisdictions' method rules not surfaced.
- Interaction with trader-class treatment (see [[trader-vs-investor]]) where mark-to-market displaces lot accounting entirely.
