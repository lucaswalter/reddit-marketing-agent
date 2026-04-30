---
title: United States
type: jurisdiction
created: 2026-04-20
updated: 2026-04-20
tags: [us, irs, federal]
sources: [[coinledger-homepage-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]]
---

## Classification

Cryptocurrency is **property** for US federal income tax purposes (per Notice 2014-21 — not explicitly cited in the CoinLedger guide but foundational to the US treatment [[coinledger-guide-united-states-2026-04-20]]). Not a currency, not a security. Stablecoins taxed the same as other crypto despite their price peg.

## Tax treatment by transaction type

- **Dispositions (sell, crypto-to-crypto trade, spend on goods/services):** capital gain/loss vs. cost basis [[coinledger-guide-united-states-2026-04-20]].
- **Mining (hobby and business), staking, airdrops, interest, hard-fork receipts, compensation:** ordinary income at FMV on receipt. Deductible business expenses only if mining-as-business (Schedule C) [[coinledger-guide-united-states-2026-04-20]].
- **Hard forks:** New coins income at FMV on receipt. (Codified in Rev. Rul. 2019-24 — to be filed as a source.) Soft forks / rebrandings: not taxable, basis carries through [[coinledger-guide-united-states-2026-04-20]].
- **DeFi lending/borrowing/LP:** No explicit IRS guidance. Conservative treatment: depositing/withdrawing liquidity is a crypto-to-crypto disposal. Yield is income [[coinledger-guide-united-states-2026-04-20]].
- **NFTs:** Treated like crypto on disposal. IRS has flagged that some NFTs (profile-pic, art) may be "collectibles" subject to the 28% collectibles gain rate [[coinledger-guide-united-states-2026-04-20]].
- **Gifts:** Not a taxable disposal. Donor lifetime exemption ~$13.99M; $19K/year per-donee annual exclusion (above → Form 709 informational). Recipient takes carryover basis [[coinledger-guide-united-states-2026-04-20]].
- **Donations:** Donating appreciated crypto held >1yr to qualified charity — no gain recognized, FMV deduction. Form 8283 if >$500 [[coinledger-guide-united-states-2026-04-20]].
- **Lost/stolen:** Not deductible post-TCJA 2017 for personal-use assets [[coinledger-guide-united-states-2026-04-20]].
- **Exchange bankruptcy (Voyager/Celsius):** Can be claimed as investment loss; doing so waives recovery right [[coinledger-guide-united-states-2026-04-20]].

## Rates and thresholds (2025 brackets)

- **Short-term (≤12mo) / ordinary income:** 10% / 12% / 22% / 24% / 32% / 35% / 37% progressive. 37% starts at $626,351 single / $751,601 MFJ [[coinledger-guide-united-states-2026-04-20]].
- **Long-term (>12mo) capital gains:** 0% / 15% / 20% progressive. 0% up to $48,350 single / $96,700 MFJ. 20% above $533,401 single / $600,051 MFJ [[coinledger-guide-united-states-2026-04-20]].

## Cost basis method

- **FIFO is default.** Specific Identification allowed — including HIFO, LIFO as Spec-ID variants — provided each disposed lot can be uniquely identified [[coinledger-guide-united-states-2026-04-20]].
- **Wallet-by-wallet basis requirement (post-2025 transition):** Historically universal-wallet tracking was acceptable; IRS guidance and 1099-DA reporting now pushes toward per-wallet tracking. Deep treatment needed in a dedicated concept page.

## Reporting forms and deadlines

- **[[form-8949]]** for individual capital-gains detail, flows to Schedule D [[coinledger-guide-united-states-2026-04-20]].
- **Schedule 1** (other income) for hobby crypto income: staking, airdrops, forks [[coinledger-guide-united-states-2026-04-20]].
- **Schedule C** for crypto business income (mining ops, contractor compensation, node operation); deductible business expenses + self-employment tax [[coinledger-guide-united-states-2026-04-20]].
- **[[form-1099-da]]** — as of 2026, all centralized exchanges issue this for customer disposals; also filed with IRS. Cost-basis fields frequently incomplete for 2025 tax year [[coinledger-guide-united-states-2026-04-20]].
- **Form 1099-MISC** for ≥$600 miscellaneous crypto income.
- **Form 1040X** to amend prior-year returns for omitted crypto.
- **Form 8283** for crypto donations >$500.
- **Deadlines:** April 15, 2026 (2025 tax year); June 15 for expats; October 15 with extension [[coinledger-guide-united-states-2026-04-20]].
- **1040 virtual-currency question:** Every US taxpayer answers under penalty of perjury [[coinledger-guide-united-states-2026-04-20]].

## Losses

- Capital losses offset **unlimited** capital gains (from any asset) + up to **$3,000/yr** of ordinary income. Excess carries forward **indefinitely** [[coinledger-guide-united-states-2026-04-20]].
- **No wash-sale rule for crypto** currently (IRC §1091 applies to "stock or securities" only — see [[tax-loss-harvesting]]). Repeated legislative proposals to extend wash-sale to digital assets have not passed as of this source.

## Regulator and primary guidance

- Primary regulator: [[irs]] (federal), under Department of the Treasury.
- State-level income taxes overlay federal in most states.
- Key guidance referenced or implied: Notice 2014-21 (property classification), Rev. Rul. 2019-24 (hard forks), Rev. Rul. 2023-14 (staking), 1099-DA broker regulations. Each deserves its own source page as primary documents are filed.

## Notable quirks

- **No wash-sale rule** for crypto — unique among major asset classes; enables tax-loss harvesting that would be disallowed on stocks.
- **1099-DA accuracy problem:** For 2025 tax year, exchanges aren't required to track/report cost basis, so the IRS and the taxpayer receive inconsistent data when crypto moves across exchanges or in/out of self-custody [[coinledger-guide-united-states-2026-04-20]]. CoinLedger's position: don't request a corrected 1099-DA, just file [[form-8949]] with correct basis from your own records.
- **Collectibles treatment for some NFTs:** Potential 28% long-term gain rate rather than the usual 20% top rate [[coinledger-guide-united-states-2026-04-20]].
- **Worldwide income taxation of citizens:** One of only two countries (with Eritrea) that taxes citizens on foreign-source income regardless of residence [[coinledger-guide-united-arab-emirates-2026-04-20]].

## Products serving US

- [[coinledger]] — primary market [[coinledger-homepage-2026-04-20]]
- Competitors: Koinly, CoinTracker, TokenTax, ZenLedger, TaxBit, Awaken, Crypto Tax Calculator (entity pages not yet created)
- Filing integrations: [[turbotax]] (official partner), [[taxact]], [[hr-block]] (desktop), [[taxslayer]]

## Gaps

- Statutory hierarchy walkthrough (statute → Treas. reg → Rev. Rul. → Notice → FAQ → court rulings).
- State-level anomalies: NY BitLicense, WA B&O, CA FTB position on crypto.
- Pre-1099-DA safe-harbor elections for basis.
- De minimis exemption legislative proposals.
- Operation Hidden Treasure, John Doe summonses.
- Wallet-by-wallet basis transition specifics (2025 cutover).
- Rev. Proc. 2024-28 (transition rules).
- Detailed guidance on margin, futures, perpetuals, prediction markets.
