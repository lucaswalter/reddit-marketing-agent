---
title: Superficial Loss Rule (Canada)
type: concept
jurisdiction: [CA]
created: 2026-04-20
updated: 2026-04-20
tags: [canada, cra, wash-sale, capital-losses]
sources: [[coinledger-guide-canada-2026-04-20]]
---

## Definition

Canada's wash-sale equivalent: a capital loss is **disallowed** if the same property (or "identical property") is reacquired within a **30-day window before or after** the disposal, and is still held at the end of the 30-day period [[coinledger-guide-canada-2026-04-20]]. The disallowed loss is added to the **Adjusted Cost Base** (see [[adjusted-cost-base]]) of the reacquired property — it is deferred, not permanently lost.

Canada's rule applies to crypto per CRA — the CRA's treatment of cryptocurrency as commodity + identical-property-pooling invokes the superficial loss framework without any crypto-specific carve-out [[coinledger-guide-canada-2026-04-20]].

## Mechanics

Statutory source: Income Tax Act s.54 ("superficial loss") and s.40(2)(g)(i) (disallowance) [primary source not yet ingested]. The 61-day window (30 before + day of + 30 after) and the "still held at end" condition both must be satisfied for the loss to be denied.

Worked example: sell 1 BTC at loss on Day 0 (proceeds $50K vs. ACB $70K → $20K loss). Rebuy 1 BTC on Day 15 at $52K. The $20K loss is disallowed; instead, the $20K is added to the new ACB → new BTC's ACB = $52K + $20K = $72K. On eventual disposal at $80K, gain = $8K vs. the $10K gain that would have arisen without the superficial-loss adjustment.

Net effect: loss is deferred into future gain reduction, not permanently lost.

## Comparison to US §1091

The Canadian rule is **stricter** than US §1091 in one respect and **identical** in mechanics:

| Dimension | Canada (superficial loss) | US (§1091) |
|---|---|---|
| Window | 30 days before + after | 30 days before + after |
| Scope | Identical property — includes crypto | "Stock or securities" — excludes crypto (see [[wash-sale-rule]]) |
| Mechanism | Loss denied, added to ACB of replacement | Loss denied, added to basis of replacement |
| Applies to crypto? | **Yes** [[coinledger-guide-canada-2026-04-20]] | No |

The key asymmetry vs. US crypto: Canadians cannot tax-loss-harvest by sell-and-immediately-rebuy. The 30-day cooling-off is real. For TLH planning, CA users must either hold the realized position for 30+ days or switch to a non-identical asset (e.g., BTC → WBTC is arguably identical; BTC → ETH is not).

## Identical-property question

CRA hasn't issued explicit guidance on what counts as "identical" for crypto [[coinledger-guide-canada-2026-04-20]]:
- **Same token on same chain:** Clearly identical (BTC ↔ BTC).
- **Wrapped/bridged equivalents:** Unclear (BTC ↔ WBTC, ETH ↔ WETH, ETH ↔ stETH). Conservative treatment: identical.
- **Different chain same token (USDC-ETH ↔ USDC-Sol):** Unclear.
- **Stablecoins pegged to same fiat:** Almost certainly not identical across issuers.

## Interaction with ACB

ACB (see [[adjusted-cost-base]]) is a running-average method, so "identical property" is already pooled. The superficial loss rule operates on the realized disposal and then adjusts the ACB of remaining units post-trigger.

## Why it matters

- **Blocks US-style crypto TLH** (see [[tax-loss-harvesting]]) — a CA user who sells BTC at a loss and rebuys within 30 days gets the loss deferred into basis rather than realized for the year.
- **Form T1A loss carryback** (3 years back / forward indefinitely) applies only to genuine realized losses — superficial-loss-deferred amounts don't qualify.
- **Spouse attribution.** ITA treats a spouse as the taxpayer for superficial-loss purposes — reacquisition by spouse within the window also triggers the rule [primary source not yet ingested].
- **Year-end planning.** December-31 losses with January reacquisition are a canonical superficial-loss trap.

## Related wiki pages

- [[adjusted-cost-base]], [[tax-loss-harvesting]], [[wash-sale-rule]], [[bed-and-breakfast-rule]], [[cost-basis-methods]], [[canada]], [[cra]].

## Primary guidance

- Income Tax Act s.54 (definition) and s.40(2)(g)(i) (disallowance) [primary source not yet ingested].
- CRA T4037 Capital Gains guide [primary source not yet ingested].

## Gaps

- No explicit CRA guidance on wrapped/bridged crypto "identical property" question.
- Treatment of DeFi swaps in-and-out of same position.
- Interaction with mining-business vs. capital treatment where loss realization is re-characterized.
