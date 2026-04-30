---
title: CARF (OECD Crypto-Asset Reporting Framework)
type: concept
jurisdiction: [global]
created: 2026-04-20
updated: 2026-04-20
tags: [oecd, carf, global-reporting, casp, information-exchange]
sources: [[coinledger-blog-dac8-eu-reporting-rules-for-crypto-asset-transactions-2026-04-20]], [[coinledger-guide-canada-2026-04-20]], [[coinledger-guide-germany-2026-04-20]]
---

## Definition

The **Crypto-Asset Reporting Framework (CARF)** is an OECD-developed automatic-exchange-of-information standard for cryptoassets, published by the OECD in October 2022 [primary source not yet ingested]. CARF is the crypto analogue of the **Common Reporting Standard (CRS)** that governs traditional financial-account information exchange between tax authorities. Participating jurisdictions commit to requiring Crypto-Asset Service Providers (CASPs) to report customer information and transactions, and to exchange that information with peer jurisdictions where customers are resident.

CARF is the **parent framework for the EU's [[dac8]]** and for Canada's 2026 CASP reporting expansion [[coinledger-guide-canada-2026-04-20]].

## Scope

Per the OECD publication [primary source not yet ingested]:

- **Who reports:** Crypto-Asset Service Providers (CASPs) — centralized exchanges, brokers, wallet services with custody, issuers doing retail distributions, and ATM operators.
- **What's reported:** User KYC data (name, address, TIN, jurisdiction of residence), aggregate transaction values by type (crypto-to-fiat, crypto-to-crypto, retail payments ≥ $50K USD threshold, transfers to unhosted wallets), and reportable annual balances.
- **To whom:** The CASP's home-jurisdiction tax authority, which then automatically exchanges with the user's residence-jurisdiction tax authority.
- **Reportable users:** Individuals and entities tax-resident in any CARF-participating jurisdiction other than the CASP's home jurisdiction.

## Timeline

- **2022-10:** OECD publishes CARF text.
- **2023:** 48 jurisdictions sign joint statement committing to CARF implementation.
- **2026:** First reporting period for most jurisdictions; first exchanges of information in 2027 [[coinledger-guide-canada-2026-04-20]].
- **2026+:** Rolling onboarding of additional jurisdictions.

Implementations in the ingested corpus:
- **Canada:** 2026 CASP reporting of fiat↔crypto, crypto↔crypto, and KYC per CARF alignment [[coinledger-guide-canada-2026-04-20]].
- **EU:** DAC8 (see [[dac8]]) is the EU's directive implementation of CARF [[coinledger-blog-dac8-eu-reporting-rules-for-crypto-asset-transactions-2026-04-20]].
- **UK:** Post-Brexit UK has signaled CARF adoption but the ingested UK guide doesn't detail timing [[coinledger-guide-united-kingdom-2026-04-20]].
- **US:** 1099-DA (see [[form-1099-da]]) is effectively the US implementation; formal CARF participation is separate and not addressed in ingested corpus.

## Relationship to jurisdictional regimes

CARF is a floor, not a ceiling. Jurisdictions layer their own rules on top:
- **EU:** DAC8 + CARF (one legal instrument, covering both domestic and cross-border).
- **Canada:** CARF + T1135 foreign-crypto reporting at CAD$100K (see [[canada]]).
- **US:** 1099-DA + FBAR (see [[fbar]]) + potentially Form 8938 → CARF participation still pending explicit adoption.

## Why it matters

- **End of non-custodial opacity for centralized venues.** Every major CEX's retail customer base becomes visible to the customer's home-jurisdiction tax authority automatically.
- **Self-custody remains outside.** CARF covers CASPs with custody or brokerage — pure self-custody wallets with no service provider don't trigger reporting. The framework treats unhosted wallets as one end of reportable transactions (CASP → unhosted), not as reporters themselves.
- **Cross-jurisdictional enforcement leverage.** A US taxpayer using KuCoin is already CARF-reportable from KuCoin's home jurisdiction → the IRS gets the data regardless of whether FBAR applies.
- **Compliance burden on CASPs.** KYC depth, transaction categorization (reportable vs non-reportable), and annual-balance reporting add engineering cost. CoinLedger positions itself as downstream of CASP data — CARF doesn't change CoinLedger's compliance footprint directly, but it does change the regulatory context for CoinLedger's CASP partners.

## Related wiki pages

- [[dac8]], [[form-1099-da]], [[fbar]], [[canada]], [[germany]], [[ireland]], [[spain]], [[sweden]], [[denmark]], [[united-kingdom]].

## Primary guidance

- OECD CARF publication (October 2022) [primary source not yet ingested].
- CARF Multilateral Competent Authority Agreement (MCAA) [primary source not yet ingested].
- Canada DAC-equivalent CASP regulations 2026 [primary source not yet ingested].

## Gaps

- Exact list of CARF-signatory jurisdictions and adoption status.
- Treatment of decentralized exchanges (DEXes) and non-custodial protocols — OECD commentary distinguishes "qualifying" CASPs; fuzzy for DeFi.
- NFT-specific treatment under CARF: in-scope for collectibles, ambiguous for utility NFTs.
- UK formal CARF adoption timing post-Brexit.
- US CARF participation status.
