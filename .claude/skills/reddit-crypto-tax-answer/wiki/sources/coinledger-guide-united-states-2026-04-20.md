---
title: CoinLedger Crypto Tax Guide — United States (2026)
type: source
created: 2026-04-20
updated: 2026-04-20
tags: [united-states, irs, guide, 1099-da, form-8949]
source_url: https://coinledger.io/guides/crypto-tax
source_type: article
author: Miles Brooks (reviewed by Jordan Bass)
publication: coinledger.io
published: 2026-04-08
last_update: 2026-04-08
ingested: 2026-04-20
raw_file: raw/guides/crypto-tax.md
---

## TL;DR

CoinLedger's master US crypto-tax guide (2026 edition). Crypto is property for federal tax purposes: dispositions trigger capital gains (short-term at 10–37% ordinary rates, long-term at 0/15/20% after a 12-month hold), and earned crypto (mining, staking, airdrops, hard forks, interest, compensation) is ordinary income at FMV on receipt. As of 2026 all centralized exchanges issue Form 1099-DA for disposals plus Form 1099-MISC for >$600 of miscellaneous income, but 1099-DA cost-basis fields are widely inaccurate — especially for cross-exchange transfers — so taxpayers must reconcile using their own records and still file [[form-8949]] themselves.

## Key claims

- **Classification:** Cryptocurrency is property, not currency or security, for federal income tax purposes. Disposals subject to capital gains tax, earnings subject to ordinary income tax.
- **Rates:** Short-term (≤1yr) gains and ordinary income taxed at 10–37% (2025 brackets reproduced). Long-term (>1yr) gains at 0/15/20% depending on income (2025 brackets reproduced).
- **Cost basis methods:** FIFO is default. Spec-ID allowed (including HIFO and LIFO as specific-identification variants) provided you can uniquely identify the disposed lot.
- **Losses:** Capital losses offset unlimited capital gains plus up to $3,000 of ordinary income per year; excess carries forward indefinitely. No wash-sale rule for crypto (still — this guide doesn't explicitly state that, but treatment is consistent with current law).
- **Form 1099-DA:** As of 2026, all centralized exchanges issue 1099-DA for disposals. Cost-basis fields on 1099-DA are commonly inaccurate during 2025 tax year because exchanges aren't required to track/report basis — transfers between exchanges break the chain. CoinLedger's position: don't request a corrected 1099-DA for basis errors; just report the correct basis on [[form-8949]] with your own records.
- **Form 1099-MISC:** Issued for ≥$600 in miscellaneous income (staking, airdrops, interest).
- **Reporting forms:** Capital gains/losses on [[form-8949]] + Schedule D. Hobby income (staking, airdrops, forks) on Schedule 1 (other income). Business crypto income (miner, node operator, contractor paid in crypto) on Schedule C — deductible expenses and self-employment tax apply.
- **Deadlines:** April 15, 2026 for 2025 tax year; June 15 for expats; October 15 with extension.
- **Staking/mining/airdrops:** Income at FMV on receipt. Subsequent disposal triggers separate capital gain/loss.
- **Hard forks:** New coins taxed as income at FMV on receipt (per Rev. Rul. 2019-24 — not cited by name in guide but implied). Soft forks/rebrands/redenominations are not taxable events; cost basis carries through.
- **DeFi:** No explicit IRS guidance for LP deposits/withdrawals; guide recommends the conservative treatment (treat LP deposit/withdrawal as crypto-to-crypto disposal). DeFi staking/yield is income.
- **NFTs:** Taxed as capital assets like other crypto on disposal; IRS has flagged that some "profile picture" / art NFTs may be collectibles subject to the 28% collectibles rate.
- **Lost/stolen crypto:** Post-TCJA 2017, personal casualty/theft losses are not deductible. Exchange-bankruptcy losses (Voyager, Celsius) may be treated as investment losses but claiming forfeits recovery rights.
- **Gifts:** Gifting is not a taxable disposal for the giver; lifetime gift-tax exemption ~$13.99M (2025), $19K annual per-donee filing threshold. Recipient takes carryover basis.
- **Donations:** Donating appreciated crypto held >1yr to a qualified charity — no capital gains recognized, deduction at FMV; Form 8283 for >$500.
- **Enforcement:** IRS works with contractors (Chainalysis) to analyze the blockchain. 1040 virtual-currency question active since 2019. Penalties for fraud: up to 5 years prison + $250K fine.

## Links

- Jurisdiction: [[united-states]]
- Regulator: [[irs]]
- Forms / concepts covered by existing pages: [[form-8949]], [[form-1099-da]], [[tax-loss-harvesting]]
- Software mentioned: [[coinledger]], [[turbotax]], [[taxact]]
