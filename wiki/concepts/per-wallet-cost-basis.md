---
title: Per-wallet cost basis (Rev. Proc. 2024-28)
type: concept
jurisdiction: [US]
created: 2026-04-20
updated: 2026-04-20
tags: [us, irs, cost-basis, rev-proc-2024-28, per-wallet]
sources: [[coinledger-blog-irs-new-crypto-cost-basis-rules-rev-proc-2024-28-2026-04-20]], [[coinledger-help-10309974-how-will-coinledger-support-new-per-wallet-cost-basis-tracking-rules-irs-rev-proc-2024-28-2026-04-20]], [[coinledger-help-10346496-2025-cost-basis-reallocation-changes-why-does-my-cost-basis-look-different-2026-04-20]], [[coinledger-help-10314185-how-do-i-change-my-cost-basis-reallocation-method-irs-rev-proc-2024-28-2026-04-20]], [[coinledger-help-10339065-how-can-i-download-a-snapshot-of-my-2025-cost-basis-reallocation-rev-proc-2024-28-2026-04-20]], [[coinledger-help-11962455-what-are-basis-reallocation-transactions-2026-04-20]], [[coinledger-help-12771568-what-is-the-reallocation-breakdown-report-2026-04-20]], [[coinledger-help-13264571-fixing-missing-cost-basis-issues-after-transitioning-to-per-wallet-cost-basis-tracking-2026-04-20]], [[coinledger-guide-united-states-2026-04-20]]
---

## Definition

US IRS **Rev. Proc. 2024-28** requires all US crypto taxpayers to track cost basis **per wallet / per account**, effective **January 1, 2025** [[coinledger-blog-irs-new-crypto-cost-basis-rules-rev-proc-2024-28-2026-04-20]]. Pre-2025 practice commonly used a **Universal** method — treating all holdings across all wallets as a single co-mingled pool for FIFO/HIFO/LIFO matching [[coinledger-blog-irs-new-crypto-cost-basis-rules-rev-proc-2024-28-2026-04-20]]. Post-2025 this is no longer permissible.

## Universal (historical)

Under Universal tracking, a disposal on Exchange B could match against the oldest lot held anywhere — even if that lot was acquired on Exchange A and never physically present at Exchange B [[coinledger-blog-irs-new-crypto-cost-basis-rules-rev-proc-2024-28-2026-04-20]]. Worked example from the CoinLedger guide: Saul holds BTC on both Exchange A (first bought at $20K) and Exchange B (later bought at $40K); sells 1 BTC from Exchange B at $50K; under Universal FIFO, the matched lot is the Exchange A $20K lot → gain $30K [[coinledger-blog-irs-new-crypto-cost-basis-rules-rev-proc-2024-28-2026-04-20]].

Universal was pragmatic pre-2025 because (a) the IRS hadn't issued contrary guidance, (b) exchanges didn't report cost basis, (c) users transferred crypto freely across venues, and (d) per-wallet tracking was operationally burdensome without software.

## Per-wallet (Rev. Proc. 2024-28)

Under per-wallet tracking, each wallet/account maintains its own independent lot inventory. The same worked example: Saul's 1-BTC sale from Exchange B now matches the Exchange B $40K lot → gain $10K. Different lot → different gain → different tax [[coinledger-blog-irs-new-crypto-cost-basis-rules-rev-proc-2024-28-2026-04-20]]. Cross-wallet transfers carry their basis with them and are non-taxable events, but the receiving wallet inherits the sending wallet's lot(s).

## The reallocation regime

For taxpayers with pre-2025 Universal-tracked history, Rev. Proc. 2024-28 creates a **basis reallocation** requirement: the historical co-mingled basis must be reallocated to specific wallets as of January 1, 2025, using one of the IRS-permitted methods [[coinledger-help-10314185-how-do-i-change-my-cost-basis-reallocation-method-irs-rev-proc-2024-28-2026-04-20]]. CoinLedger surfaces the reallocation decision to the user and generates:

- **Basis reallocation transactions** — synthetic ledger entries representing the allocation of historical basis to specific wallets [[coinledger-help-11962455-what-are-basis-reallocation-transactions-2026-04-20]].
- **Reallocation Breakdown Report** — auditor-ready summary showing how historical universal pools were split per wallet [[coinledger-help-12771568-what-is-the-reallocation-breakdown-report-2026-04-20]].
- **2025 snapshot download** — point-in-time record for safe-harbor documentation [[coinledger-help-10339065-how-can-i-download-a-snapshot-of-my-2025-cost-basis-reallocation-rev-proc-2024-28-2026-04-20]].

CoinLedger support has explicit articles acknowledging that **reallocated numbers will look different** from prior-year outputs — a material UX moment for users doing year-over-year comparisons [[coinledger-help-10346496-2025-cost-basis-reallocation-changes-why-does-my-cost-basis-look-different-2026-04-20]].

## Practical implications

- **Software migration is load-bearing.** The migration generates new [[missing-cost-basis]] warnings at wallets that had no first-inflow context under the Universal view but are now tracked standalone [[coinledger-help-13264571-fixing-missing-cost-basis-issues-after-transitioning-to-per-wallet-cost-basis-tracking-2026-04-20]].
- **Reported numbers can go up or down.** Depending on which wallets held high-basis vs low-basis lots, reallocation can either raise or lower realized gain on 2025 dispositions.
- **1099-DA alignment.** Per-wallet basis aligns with how brokers will report under [[form-1099-da]] — exchange A's 1099-DA will show basis for lots acquired at exchange A, not lots that once lived at exchange B. Pre-Rev-Proc-2024-28 Universal numbers would mismatch the 1099-DA structurally.
- **Safe harbor window.** Rev. Proc. 2024-28 provides a transition safe harbor for reasonable allocation methods applied consistently [[coinledger-help-10309974-how-will-coinledger-support-new-per-wallet-cost-basis-tracking-rules-irs-rev-proc-2024-28-2026-04-20]] [primary source not yet ingested — full Rev. Proc. text].

## Related wiki pages

- [[cost-basis-methods]], [[spec-id]], [[missing-cost-basis]], [[form-1099-da]], [[form-8949]], [[united-states]], [[irs]].

## Primary guidance

- Rev. Proc. 2024-28 [primary source not yet ingested].
- Treas. Reg. §1.1012-1(j) [primary source not yet ingested].

## Gaps

- Exact permitted reallocation methods under the safe harbor — not detailed in ingested blog/help.
- Treatment of self-custody wallets vs. exchange accounts under "per wallet" — is each seed-phrase a wallet, or each derivation path?
- Interaction with DeFi protocol "accounts" where beneficial ownership is ambiguous.
- Whether other jurisdictions will follow the US per-wallet shift.
