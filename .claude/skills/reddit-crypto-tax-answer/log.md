# Wiki Log

Append-only. Every entry starts with `## [YYYY-MM-DD] <op> | <title>` so `grep "^## \[" log.md | tail -20` returns a clean timeline.

Ops: `ingest` · `query` · `lint` · `schema` · `refactor`

---

## [2026-04-20] schema | Initialized wiki

- Created `CLAUDE.md` schema for crypto-tax LLM Wiki (domain: crypto taxation, CoinLedger + competitors, regulatory landscape).
- Scaffolded directories: `raw/`, `raw/assets/`, `wiki/sources/`, `wiki/entities/`, `wiki/concepts/`, `wiki/jurisdictions/`, `wiki/comparisons/`, `wiki/syntheses/`.
- Created `index.md` (empty catalog) and `log.md` (this file).
- Conventions set: kebab-case slugs, YAML frontmatter on every page, inline `[[source-slug]]` citations, explicit contradiction handling, jurisdictional tagging required on tax claims, lint is report-only (no auto-fix).
- Ready for first ingest.

## [2026-04-20] ingest | CoinLedger homepage + pricing page

- Source: https://coinledger.io/ (+ /pricing), fetched via WebFetch. Raw saved to `raw/coinledger-homepage-2026-04-20.md` (extracted content, not literal HTML — note on provenance in the file).
- Source page: `wiki/sources/coinledger-homepage-2026-04-20.md`.
- Created full entity page: [[coinledger]] — positioning, scale claims, integration surface, pricing table, service flows, jurisdictions, open questions.
- Created stubs: [[turbotax]], [[taxact]], [[hr-block]], [[taxslayer]], [[irs]] (entities); [[form-8949]], [[form-1099-da]], [[tax-loss-harvesting]] (concepts); [[united-states]], [[germany]] (jurisdictions).
- Flagged inconsistencies for future reconciliation: (1) homepage "100+ exchanges / 60+ wallets / 30+ chains" vs. pricing page "1,000+ integrations" — definitional basis differs; (2) Pro tier "$199+" overage pricing not exposed; (3) DFY/White-Glove pricing opaque; (4) TurboTax "Official Partner" arrangement undated/undocumented.
- No contradictions with prior wiki state (first ingest).
- Index updated.

## [2026-04-20] schema | Bulk-ingest mode amendment

- Added "Bulk ingest" section to CLAUDE.md ahead of the 490-source CoinLedger run.
- Rules: no new stubs during bulk (flag for Lucas instead); lighter source-page template; one inventory synthesis per collection; infrastructure exceptions OK (regulators, jurisdictions); one log entry per phase.

## [2026-04-20] ingest | Phase 1 — 14 CoinLedger jurisdictional guides

- Source: https://coinledger.io/guides/*. Scraped via Firecrawl CLI → `raw/guides/*.md`. Raw artifacts are full-page markdown.
- 14 source pages filed under `wiki/sources/coinledger-guide-*-2026-04-20.md`.
- 12 new jurisdiction pages created (australia, canada, denmark, india, ireland, japan, new-zealand, south-africa, spain, sweden, united-kingdom, united-arab-emirates); 2 existing stubs enriched with real content ([[united-states]], [[germany]]).
- 13 new regulator entity pages created: [[ato]], [[cra]], [[skattestyrelsen]], [[bzst]], [[cbdt]], [[revenue-ireland]], [[nta-japan]], [[ird-new-zealand]], [[sars]], [[aeat]], [[skatteverket]], [[hmrc]], [[fta-uae]]. ([[irs]] pre-existed.)
- Delegated per-source filing to a general-purpose subagent; all 14 guides processed in one agent run. Every jurisdiction page built to the established pattern (classification, transaction treatment, rates, cost-basis, forms, losses, regulator, quirks, gaps).
- Contradiction flagged: UK CGT allowance cited inconsistently in the source (£3,000 for 2024-25 vs. £6,000 — latter appears stale). Noted in [[coinledger-guide-united-kingdom-2026-04-20]].
- Minor source-level correction: India guide's typo calling CBDT "IRS" was silently fixed in the source page.
- No new concept pages created (per bulk amendment). Substantial concept gaps flagged for Lucas in final report — see `wiki/syntheses/` and CLAUDE.md schema for the prioritized backlog.

## [2026-04-20] ingest | Phase 2 — 151 CoinLedger blog posts

- Source: https://coinledger.io/blog/*. Scraped via Firecrawl CLI → `raw/blog/*.md`.
- 151 source pages filed under `wiki/sources/coinledger-blog-*-2026-04-20.md` using the lighter bulk template (TL;DR + 3-5 key claims + tags + signal tier).
- Inventory synthesis created: [[coinledger-blog-inventory-2026-04-20]] — topical distribution, by-jurisdiction/by-transaction-type/by-exchange groupings, content-marketing patterns, 5 standouts, gaps.
- Signal tiers: 25 high / 100 medium / 26 low.
- Dominant 2026 editorial push: Form 1099-DA (18 posts). Heaviest jurisdictional concentration: US (129 of 151).
- No new concept/entity/jurisdiction stubs created (per bulk amendment). Strong backlog flagged: form-1099-b/1099-misc/1099-k, FBAR, Rev. Proc. 2024-28, Notice 2014-21, IIJA broker provisions, per-wallet-cost-basis, defi-tax-treatment, staking-rewards, nft-tax-treatment concepts; portugal/brazil/singapore/puerto-rico jurisdictions; exchange/competitor/people entities.
- Delegated to general-purpose subagent; one agent run.

## [2026-04-20] ingest | Phase 3 — 324 CoinLedger help-center articles

- Source: https://help.coinledger.io/en/articles/*. Scraped via Firecrawl CLI → `raw/help/*.md`.
- 324 source pages filed under `wiki/sources/coinledger-help-*-2026-04-20.md` using the lightest bulk template (1-sentence TL;DR + 2-4 bullets + tags + signal tier).
- Inventory synthesis created: [[coinledger-help-inventory-2026-04-20]] — full integration coverage list (91 exchanges, 22 wallets, 51 chains, 5 on-chain protocols), most-complex support themes, legacy cruft, product-complexity patterns.
- Signal tiers: 63 high / 229 medium / 32 low.
- **Reconciliation finding:** The help-article floor is 91 exchanges / 22 wallets / 51 chains — well below the homepage's "100+/60+/30+" and nowhere near pricing page's "1,000+ integrations." Long tail is served by universal-CSV + wallet-address imports, not dedicated articles. Previously-flagged marketing inconsistency now has a concrete counting basis.
- Most complex product themes surfaced: Missing Cost Basis warnings (9+ articles, 11-cause taxonomy), Rev. Proc. 2024-28 per-wallet migration, Form 8949 correctness math, transaction-classification UI (Uncategorized / PBT tab), import-failure triage.
- Legacy cruft documented: Coinbase Pro, Bittrex, Mandala, Graviex, AnchorUSD, Terra/Luna, Voyager, ShapeShift still have help pages (no legacy flag). URL bifurcation to `help.cryptotrader.tax` still present post-2022 rebrand.
- Authorship: Benjamin Yoder (support/import), David Kemmerer (co-founder, infra pieces), Lucas Wyland (pricing, chains list).
- Delegated to general-purpose subagent; one agent run.
- No new stubs created (per bulk amendment). Massive concept/entity backlog flagged — in particular CoinLedger-specific product concepts that only appear in help (missing-cost-basis, per-wallet-cost-basis, potential-bridges-trades-transfers, universal-import-template, reallocation-breakdown-report, etc.) and the long list of exchange/wallet/chain entities referenced across the help corpus.

## [2026-04-20] refactor | Concept backlog buildout — 24 new concept pages

- Approved by Lucas after Phase 3 ingest report. Delegated to general-purpose subagent with tight source-grounding requirements.
- Created 24 concept pages grouped across five areas:
  - **US forms (5):** [[form-1099-b]], [[form-1099-k]], [[form-1099-misc]], [[fbar]]; existing [[form-8949]] and [[form-1099-da]] kept.
  - **US tax doctrine (8):** [[wash-sale-rule]], [[cp2000]], [[hard-fork-taxation]], [[airdrop-taxation]], [[staking-rewards]], [[defi-tax-treatment]], [[nft-tax-treatment]], [[trader-vs-investor]].
  - **Cost basis (4):** [[cost-basis-methods]] (umbrella), [[per-wallet-cost-basis]], [[spec-id]], [[missing-cost-basis]] (CoinLedger product concept).
  - **Jurisdiction-specific (4):** [[shared-pool-accounting]] (UK), [[bed-and-breakfast-rule]] (UK + SA), [[superficial-loss-rule]] (CA), [[adjusted-cost-base]] (CA).
  - **Global regulatory (2):** [[carf]], [[dac8]].
  - **CoinLedger product (2):** [[potential-bridges-trades-transfers]], [[universal-import-template]].
- Total concepts now: 27 (3 original + 24 new).
- Every page uses inline `[[source-slug]]` citations; primary IRS guidance (Notice 2014-21, Rev. Ruls., Rev. Proc. 2024-28) marked `[primary source not yet ingested]` consistently across pages — no fabricated citations.
- **Contradictions flagged during concept authoring:**
  - Airdrop receipt (US) — guide says ordinary income regardless of active/passive; airdrop blog doesn't address valuation-timing nuance for retroactive claims.
  - Canada airdrops — guide is internally ambiguous ($0-basis-new-asset vs. income-like-hard-forks).
  - Staking dominion-and-control doctrine (Rev. Rul. 2023-14) nowhere explicit in CoinLedger sources — added as primary-not-yet-ingested.
  - UK bed-and-breakfast directionality — guide blurs "30 days before and after" vs. statute's 30-days-post-only (TCGA s.106A). Worth a lint check.
- **Pages with thin source coverage (flagged for deeper sourcing):** [[carf]], [[spec-id]], [[universal-import-template]], [[potential-bridges-trades-transfers]], [[fbar]].
- **Next-up backlog surfaced during authoring:** 5 legislation/entity pages urgently needed — Rev. Proc. 2024-28, Rev. Rul. 2019-24, Rev. Rul. 2023-14, Notice 2014-21, OECD CARF (primary). Close also-ran: IIJA broker provisions.
- Index updated; `wiki/concepts/` section restructured into 6 sub-groupings.
