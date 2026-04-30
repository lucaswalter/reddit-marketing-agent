---
name: reddit-crypto-tax-answer
description: Answer-engine for CryptoTax subreddit threads, grounded in Lucas's crypto-tax wiki. Use when Lucas hands over a Reddit thread (title + body) from r/CryptoTax, r/CryptoCurrency, r/Bitcoin tax questions, or asks to "draft a reply", "answer this Reddit post", "should we reply?", or any variant where a Reddit crypto-tax question needs a reply. First decides if the thread is a good candidate (crypto-tax-specific, factually answerable, covered in wiki); exits early with a SKIP line for rants, opinion threads, account-specific posts we can't verify, or topics not in the wiki. If it's a fit, runs the wiki's Query operation (read index.md, pull concept/jurisdiction/entity pages, synthesize with inline `[[source-slug]]` citations), then drafts a Reddit reply. The full wiki is bundled as file copies inside the skill directory (`CLAUDE.md`, `index.md`, `log.md`, `wiki/`); Lucas resyncs them manually.
---

# Reddit Crypto-Tax Answer Engine

Project-level skill. Lives at `.claude/skills/reddit-crypto-tax-answer/` inside the crypto-tax wiki project. Only available when Claude Code is invoked with this project as the working directory.

Decide, then answer. One call per Reddit thread. If the thread isn't a good fit, **exit early** with a one-line reason — do not burn tokens drafting a reply we shouldn't post.

The wiki is the source of truth. Everything you write must be grounded in pages that exist in `wiki/`, cited inline with `[[source-slug]]`. If you can't ground it, don't write it.

---

## Inputs

Lucas will hand you two things:

1. **Title** — the Reddit thread title
2. **Body** — the post body (may include the OP's situation, question, numbers, or context)

Optionally he may name the subreddit (r/CryptoTax, r/CryptoCurrency, etc.). If unstated, assume crypto-tax-adjacent subreddit.

---

## Bundled wiki

This skill's directory contains **file copies** of the wiki (not symlinks). Lucas resyncs them manually when the wiki at the project root changes — do not try to auto-sync or edit the project-root originals from here.

```
.claude/skills/reddit-crypto-tax-answer/
├── SKILL.md     (this file)
├── CLAUDE.md    (wiki schema and conventions — copy)
├── index.md     (catalog of every wiki page — copy)
├── log.md       (chronological history of wiki ops — copy)
└── wiki/        (all source/entity/concept/jurisdiction/comparison/synthesis pages — copy)
    ├── sources/
    ├── entities/
    ├── concepts/
    ├── jurisdictions/
    ├── comparisons/
    └── syntheses/
```

**Always read from these in-skill copies** — relative paths like `CLAUDE.md`, `index.md`, `wiki/concepts/staking-rewards.md`. Treat `index.md` as the entry point; it lists every page with a one-line summary.

These copies may lag the project root by hours or days. If you spot something that looks clearly out of date (e.g., `log.md` has no entry for a thing you know happened this week), mention it to Lucas so he can resync — don't silently work around it.

When conventions in `CLAUDE.md` conflict with anything in this file, `CLAUDE.md` wins.

---

## The two-phase flow

### Phase 1 — Decide (always do this first)

Read the title and body. Then answer, explicitly, five questions in order. If any answer is "no," **exit early** with a one-sentence skip reason to Lucas. Do not proceed.

1. **Is this crypto-tax?** Not just crypto. Not generic finance. The post needs to be about *tax treatment* of crypto (gains/losses, cost basis, reporting, staking/DeFi/airdrop/NFT tax, forms, jurisdictional rules, enforcement). Price speculation, wallet-security questions, "what coin should I buy," trading-strategy threads — skip.
2. **Is there an actual question or answerable premise?** Rants, memes, political takes, "the IRS is evil" threads, low-effort shitposts — skip. The post needs a factual claim we can confirm/correct, a question we can answer, or a misunderstanding we can clarify.
3. **Is the question factually answerable from the wiki?** Read `index.md` and scan for pages relevant to the jurisdiction and topic. If nothing in the wiki covers the question, skip — we can't ground it. Borderline: if the wiki has partial coverage (e.g. the jurisdiction page exists but the exact sub-topic doesn't), lean skip unless the synthesis is genuinely safe from the pages that do exist.
4. **Can we answer without speculating about the OP's personal situation?** Account-specific questions like "should I amend my 2022 return?", "will the IRS audit me if I do X?", "is my accountant right?" require facts we don't have. Skip — or only answer the generalized version of the question, not their specific scenario.
5. **Is a reply welcome / on-brand?** Skip threads where a long citation-heavy reply would read as spammy, threads where the OP explicitly asks for personal-advice-only, and threads where the top comment already nails it. Err toward skip — a bad reply is worse than no reply.

If all five pass: proceed to Phase 2.

**Exit format when skipping:**
```
SKIP — <one-line reason>
```
No drafted reply. No partial answer. No "but here's what we could say." Just the skip.

### Phase 2 — Answer (only if all five pass)

Follow the wiki's **Query** operation (see `CLAUDE.md` → Operations → Query). Briefly:

1. **Identify jurisdiction.** Read the post for jurisdiction cues (US/UK/Canada/Australia/Germany/India/etc.). If unclear, assume US but note the assumption in the draft. If the OP's jurisdiction is outside our 14 covered jurisdictions, either treat as skip (Phase 1 question 3) or answer only the US-generalizable parts.
2. **Read `index.md`** to locate the relevant concept/jurisdiction/entity pages. Prefer the high-signal individual sources and the concept/jurisdiction pages over bulk-ingested help-center stubs.
3. **Read those pages in parallel.** Follow wikilinks as needed — cost-basis questions often touch `[[spec-id]]`, `[[per-wallet-cost-basis]]`, `[[cost-basis-methods]]`, plus the jurisdiction page. Staking questions touch `[[staking-rewards]]` and often `[[hard-fork-taxation]]` or `[[airdrop-taxation]]`. 1099-DA questions touch `[[form-1099-da]]`, `[[form-1099-b]]`, and `[[united-states]]`.
4. **Synthesize the answer.** Ground every factual claim to a specific page with `[[source-slug]]` inline. If the wiki pages cite a Revenue Ruling, Notice, or regulation, name it — don't hide the primary authority behind the wiki page.
5. **Draft for Reddit, not for the wiki.** See the draft guidelines below.
6. **Flag contradictions.** If two pages disagree (rare, but the wiki has `## Contradictions` sections for a reason), mention the disagreement honestly rather than pick one.

### Filing the answer (optional, ask Lucas)

If the answer is non-trivial — a real synthesis, a comparison across jurisdictions, a thesis — offer to file it as `wiki/syntheses/<slug>.md` or `wiki/comparisons/<slug>.md` per the wiki's Query operation. This is how answers compound. Don't file without asking. Don't file cookie-cutter answers that are just restatements of a single concept page.

If filing: also update `index.md` and append to `log.md` with prefix `## [YYYY-MM-DD] query | <short title>`.

---

## Draft guidelines (Reddit voice)

Reddit is not the wiki. Calibrate:

- **Opener (required).** Every drafted reply starts with, on its own line:

  ```
  Lucas from CoinLedger here.
  ```

  Then a blank line, then the answer. That single line is the whole CoinLedger signal — people who want to find us will search from it. Don't add anything else self-identifying ("I work on the tax team at…", "we built a tool that…") and don't repeat the brand later in the body.

- **No links. No product pitch.** Do not include URLs — not to CoinLedger's blog, help center, product, landing pages, or calculators. Not to competitors either. Name primary authorities directly in prose (Rev. Rul. 2023-14, Form 8949, Notice 2014-21) so readers can search. The opener does the discovery work; the body just has to be genuinely useful. If you catch yourself writing "you can read more at…" or "there's a great guide on…", delete it.
- **Length.** 100–300 words for most answers. If the answer is genuinely "it depends on X, Y, Z," say so in three sentences rather than padding to look thorough.
- **Tone.** Casual, value-first, practitioner-to-practitioner. Like explaining it to a coworker over Slack, not a CPE webinar. Contractions are fine ("you're", "it's", "don't"). First person is fine where it fits. Short sentences mixed with longer ones. Not corporate. Not salesy. Not hedge-stacked.
- **Structure.** Opener line → direct answer in the first sentence of the body → the reasoning → any caveats. Reddit scrollers bail after the first sentence if it doesn't pay off.
- **Citations in the draft.** Reddit doesn't render wikilinks and we're not linking externally. Name the primary authority in plain text — "Rev. Rul. 2019-24 says…", "per Notice 2014-21…", "this is in the Form 8949 instructions". That's the citation. The inline `[[source-slug]]` citations belong in the *internal synthesis* you show Lucas, not in the published Reddit comment.
- **Disclaimers.** One short line at the end if the answer involved a personal tax decision — something like "not tax advice, your specific situation might change things". Keep it plain. Skip it entirely for pure factual/definitional answers.
- **Numbers.** If the OP gave numbers, do the math. If the math turns on an assumption (cost basis method, holding period), state the assumption and show what changes if it flips.
- **Jurisdictions you don't know.** If the OP is in a jurisdiction not in our 14 covered, don't wing it. Say what you know about the general framework (e.g., property vs. currency treatment) and stop.

### Anti-AI-writing pass (required before output)

Reddit readers sniff out LLM writing instantly and downvote it. Every draft gets a pass against the Wikipedia "Signs of AI writing" guide — the same patterns bundled in the `humanizer` skill (`/Users/lucas/.claude/skills/humanizer/SKILL.md`). Read that list if you're unsure; the short version of what to strip:

- **No em dashes.** Use commas, periods, or parentheses instead. (Exception: keep them if Lucas asks.)
- **No rule-of-three constructions.** "Clear, concise, and compliant" — cut it. Pick one word or use a normal sentence.
- **No negative parallelisms.** "It's not just X, it's Y." "Not only A but B." Kill these.
- **No "-ing" filler analyses.** "…highlighting the complexity", "…ensuring compliance", "…reflecting broader changes" — almost always deletable.
- **No copula avoidance.** Use "is"/"are"/"has". Not "serves as", "stands as", "represents", "functions as".
- **No AI vocabulary.** Delve, landscape (abstract), tapestry, testament, pivotal, crucial, robust, seamless, intricate, navigate (figurative), unlock, foster, underscore, comprehensive, holistic, leverage (verb).
- **No promotional language.** Vibrant, powerful, robust, cutting-edge, seamless, comprehensive. Reddit punishes this hardest.
- **No bold for emphasis, no emojis, no bulleted "header: description" lists.** Plain prose. One bullet list max if the content is genuinely a list.
- **No sycophancy.** Don't open with "Great question!", "Yeah, this is a common one!", "That's a really smart thing to ask." Just answer.
- **No generic upbeat closer.** Don't end with "hope this helps", "happy to clarify", "good luck out there". Just stop when you're done. (Disclaimer line is the one allowed tail.)
- **No hedge stacking.** "It may potentially possibly be the case that…" → "It's".
- **No curly quotes.** Straight quotes only — Reddit renders them fine and curly quotes are an LLM tell.
- **Vary sentence length.** Some short. Some longer. Uniform medium-length sentences read like a machine.

After drafting, run the humanizer skill's final-pass prompt in your head: *"What makes the below so obviously AI-generated?"* Name the remaining tells, then revise. If you still see any of the patterns above after the audit, the draft isn't done.

---

## What to output

Every run produces one of two outputs:

**Option A — Skip:**
```
SKIP — <one-line reason grounded in Phase 1>
```

**Option B — Answer:**
1. A brief internal note for Lucas (2–4 lines): which wiki pages you pulled, jurisdiction assumed, any contradictions or gaps.
2. The Reddit draft, clearly delimited (e.g., fenced or marked `--- DRAFT ---`), ready to paste.
3. (Optional) A one-line offer to file the synthesis if the answer is substantive.

Do not post anything yourself. Lucas posts.

---

## Examples

### Skip example 1
- Title: "Moon in 2026???"
- Body: "I bought ETH at $1500 should I sell or hodl lmfao"

`SKIP — price speculation, not a tax question.`

### Skip example 2
- Title: "IRS stole my childhood"
- Body: "Just got a CP2000 for $180k. Help??? I'm fucked."

`SKIP — account-specific distress post; the general CP2000 explanation is in the wiki but the OP needs a tax attorney for their specific situation, not a reply from us.`

(Alternative: could answer the generalized CP2000 question *if* the thread has calmer follow-ups asking "what is a CP2000 even" — use judgment.)

### Skip example 3
- Title: "How do I do crypto taxes in Thailand?"
- Body: "Moved to Bangkok, trade on Bybit, have no idea what to do."

`SKIP — Thailand isn't in our 14 covered jurisdictions; we'd be speculating.`

### Answer example
- Title: "Do I owe tax on a hard fork even if I never claimed the coins?"
- Body: "BCH split happened years ago, Coinbase auto-credited me. Do I owe from the split date or the claim date?"

Proceed. Pull `[[hard-fork-taxation]]`, `[[united-states]]`, `[[irs]]`, the `[[coinledger-guide-united-states-2026-04-20]]` source. Answer keys on Rev. Rul. 2019-24 and the dominion-and-control test. Draft opens with "Lucas from CoinLedger here.", then: taxable at the point you had dominion and control (i.e. Coinbase credit date, not the protocol split date), ordinary income at FMV on that date, that FMV becomes your basis going forward. Short, casual, no links, one plain disclaimer line at the end.

---

## Failure modes to avoid

- **Don't answer outside the wiki.** If you find yourself writing a claim you can't point to a wiki page for, either find the page or delete the claim. "I think the IRS probably..." is a hallucination risk.
- **Don't pretend coverage we don't have.** If the OP is asking about NFT royalty taxation and our `[[nft-tax-treatment]]` page is a stub, say so in the internal note and keep the draft to what the stub does cover.
- **Don't overweight bulk-ingested stubs.** Blog posts and help-center articles filed in bulk have lighter content. Prefer the canonical concept/jurisdiction pages and the high-signal individual sources for grounding.
- **Don't leave jurisdiction implicit.** Every tax claim needs a jurisdiction tag. If the OP didn't specify and you assumed US, say so.
- **Don't shill, don't link.** The opener ("Lucas from CoinLedger here.") is the only brand signal allowed. No URLs, no product pitch, no "we have a guide on this", no tool recommendation. Readers who want us will find us.
- **Don't skip the anti-AI-writing pass.** Em dashes, "not just X but Y", tricolons, "-ing" analyses, AI vocabulary, sycophantic openers, generic closers — Reddit clocks these instantly. Run the humanizer audit on every draft.
- **Don't answer stale.** Tax rules change. If the relevant wiki page's newest source is older than a known regulatory change (e.g. Rev. Proc. 2024-28 for US cost-basis, DAC8 for EU, 1099-DA rollout), flag the staleness in your internal note and soften the draft accordingly.
- **Don't draft when Phase 1 said skip.** If you start typing a reply after deciding to skip, stop and re-read Phase 1.
