---
title: DAC8 (EU Directive 2023/2226)
type: concept
jurisdiction: [EU]
created: 2026-04-20
updated: 2026-04-20
tags: [eu, dac8, carf, casp, information-exchange]
sources: [[coinledger-blog-dac8-eu-reporting-rules-for-crypto-asset-transactions-2026-04-20]], [[coinledger-guide-germany-2026-04-20]], [[coinledger-guide-ireland-2026-04-20]], [[coinledger-guide-spain-2026-04-20]], [[coinledger-guide-sweden-2026-04-20]], [[coinledger-guide-denmark-2026-04-20]]
---

## Definition

**DAC8** is the 8th amendment to the EU Directive on Administrative Cooperation — formally Council Directive 2023/2226 — adopted October 17, 2023 [primary source not yet ingested]. DAC8 is the EU's legal implementation of the OECD's [[carf]] [[coinledger-blog-dac8-eu-reporting-rules-for-crypto-asset-transactions-2026-04-20]]. It imposes CASP (Crypto-Asset Service Provider) reporting obligations for both **domestic and cross-border** EU transactions.

Go-live: **January 1, 2026** [[coinledger-blog-dac8-eu-reporting-rules-for-crypto-asset-transactions-2026-04-20]], [[coinledger-guide-germany-2026-04-20]]. First reports cover the 2026 calendar year; first exchanges between member-state tax authorities in 2027.

## Scope

Per the directive [[coinledger-blog-dac8-eu-reporting-rules-for-crypto-asset-transactions-2026-04-20]]:

- **Reporting CASPs:** Any platform offering buy/sell/trade services for crypto-assets to EU residents, regardless of where the CASP is based. Explicit extraterritorial reach.
- **User KYC captured at signup:** Name, address, tax identification number, date of birth, jurisdiction of residence.
- **Reportable transactions:**
  - Crypto ↔ fiat exchanges.
  - Crypto ↔ crypto exchanges.
  - Retail crypto-for-goods/services transactions ≥ EUR 50,000 per transaction.
  - Transfers to/from unhosted wallets (with balance/volume aggregation).
- **Frequency:** Annual.

CASPs report to their home member-state tax authority, which then exchanges data with the user's residence member state.

## Jurisdictions in the ingested corpus that reference DAC8

The CoinLedger jurisdiction guides explicitly call out DAC8 as go-live January 2026 for:
- **Germany** [[coinledger-guide-germany-2026-04-20]]
- **Ireland** [[coinledger-guide-ireland-2026-04-20]]
- **Spain** [[coinledger-guide-spain-2026-04-20]]
- **Sweden** [[coinledger-guide-sweden-2026-04-20]]
- **Denmark** [[coinledger-guide-denmark-2026-04-20]]

Other EU member states (France, Italy, Netherlands, Belgium, Portugal, Austria) are equally in-scope but lack dedicated ingested guides.

## Relationship to CARF

DAC8 = CARF-aligned + extra EU teeth:
- **DAC8 covers intra-EU domestic CASPs** — the OECD CARF MCAA is inherently cross-border, but DAC8 captures an Irish resident using an Irish CASP (which MCAA alone wouldn't trigger).
- **Penalty regime** is EU-harmonized via the directive — member states must provide "effective, proportionate, and dissuasive" penalties for non-compliance.
- **Interaction with MiCA:** DAC8 reporting overlays the EU's Markets in Crypto-Assets licensing regime. CASPs that are MiCA-licensed are presumed DAC8 reporters.

See [[carf]] for the broader framework and non-EU implementations.

## Why it matters

- **Retroactive KYC at EU exchanges.** Users who signed up pre-DAC8 without full tax-ID disclosure are being re-prompted at go-live. This is the visible UX moment for DAC8 enforcement.
- **Non-EU exchanges serving EU customers** (Binance.com, KuCoin, OKX) are technically in-scope extraterritorially — enforcement is unclear but the statutory hook exists.
- **Crypto tax software downstream effect.** CoinLedger / competitor users in DAC8 jurisdictions get richer tax-authority visibility into their on-platform activity. Platforms serving Germany/IE/ES/SE/DK need to anticipate users receiving matching-notices analogous to US [[cp2000]].
- **End of un-flagged small-transaction anonymity.** DAC8 has no de minimis for domestic reporting — every transaction by an EU-resident CASP customer is reportable.

## Related wiki pages

- [[carf]], [[fbar]], [[form-1099-da]], [[cp2000]], [[germany]], [[ireland]], [[spain]], [[sweden]], [[denmark]].

## Primary guidance

- Council Directive (EU) 2023/2226 of 17 October 2023 amending Directive 2011/16/EU on administrative cooperation in the field of taxation [primary source not yet ingested].
- OECD CARF [primary source not yet ingested] — parent framework.
- MiCA (Regulation (EU) 2023/1114) [primary source not yet ingested] — licensing overlay.

## Gaps

- Full list of DAC8-scoped transaction types (the directive's Annex VI is not in ingested corpus).
- Enforcement posture for non-EU CASPs that ignore DAC8.
- Member-state variance in penalty regimes.
- Treatment of DeFi / non-custodial protocols vs. custodial CASPs.
- Interplay with VAT-on-crypto-services (Ireland is unusual — see [[ireland]]).
