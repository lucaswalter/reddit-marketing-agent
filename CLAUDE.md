# CLAUDE.md — Crypto Tax LLM Wiki Schema

This directory is an **LLM Wiki** (second brain) for **cryptocurrency taxation, digital asset tax policy, and CoinLedger product/competitor context**. Ignore the directory name (`reddit-marketing-agent`) — it is misleading. Lucas works at CoinLedger (`lucas@coinledger.io`); assume strong domain knowledge.

You are the wiki maintainer. Lucas curates sources and asks questions; you do all the reading, filing, cross-referencing, and bookkeeping.

---

## Layers

1. **`raw/`** — immutable source documents Lucas drops in (articles, PDFs, screenshots, pastes, transcripts). Never modify. Images and attachments go under `raw/assets/`.
2. **`wiki/`** — LLM-authored markdown. You own this layer entirely.
3. **`index.md` + `log.md`** — navigation and history. Update on every operation.
4. **`CLAUDE.md`** (this file) — schema. Co-evolves with Lucas. Update it when conventions change.

---

## Directory layout

```
raw/                      # immutable sources
  assets/                 # images, PDFs, screenshots
wiki/
  sources/                # one page per ingested source
  entities/               # companies, products, people, agencies (CoinLedger, Koinly, IRS, Treasury, etc.)
  concepts/               # tax concepts (cost basis, wash sales, staking rewards, DeFi treatment, etc.)
  jurisdictions/          # US, UK, EU, Canada, Australia, India, etc. — per-country tax regime pages
  comparisons/            # competitor feature matrices, regime comparisons, method comparisons
  syntheses/              # topic deep-dives, theses, analysis pages born from queries
index.md                  # content catalog (category-organized)
log.md                    # chronological operation log
CLAUDE.md                 # this schema
```

Page slugs: `kebab-case.md`. Wikilinks use `[[page-name]]` (Obsidian-compatible).

---

## Page conventions

Every wiki page starts with YAML frontmatter:

```yaml
---
title: <human-readable title>
type: source | entity | concept | jurisdiction | comparison | synthesis
created: YYYY-MM-DD
updated: YYYY-MM-DD
tags: [tag1, tag2]
sources: [[source-slug-1]], [[source-slug-2]]   # pages this page draws from (non-source types)
---
```

**Source pages** additionally carry:
```yaml
source_url: <original URL if applicable>
source_type: article | paper | podcast | video | regulation | filing | paste | screenshot | transcript
author: <if known>
publication: <if known>
published: YYYY-MM-DD
ingested: YYYY-MM-DD
raw_file: raw/<filename>
```

**Entity pages** additionally carry:
```yaml
entity_kind: company | product | person | agency | court | legislation
jurisdiction: [US, UK, ...]   # if scoped
```

**Body structure (guideline, not rigid):**
- Source pages: one-paragraph TL;DR → key claims (bulleted, each with implications) → quotes worth keeping → entities/concepts touched (wikilinks) → open questions.
- Entity/concept/jurisdiction pages: definition → current state → key facts with inline source citations `[[source-slug]]` → history/evolution → related pages → contradictions-in-sources (if any).
- Comparisons: frontmatter + table + short per-cell footnote with citations.
- Syntheses: thesis → evidence → counterevidence → confidence → what would update this.

**Citations**: inline wikilinks to source pages, not URLs. The source page carries the URL.

**Contradictions**: when a new source contradicts an existing claim, don't overwrite. Add a `## Contradictions` section on the affected page with both claims and their sources, then flag it in the ingest report.

---

## Operations

### Ingest

When Lucas drops a new source:

1. **Save raw.** Copy/save to `raw/<slug>.<ext>` (or `raw/assets/` for images). If it's a paste, save as `raw/<slug>.md`. Never modify after this.
2. **Read it fully.** For images referenced in markdown, read them with the Read tool in a second pass.
3. **Discuss briefly.** Surface 2–5 key takeaways to Lucas before filing. He may redirect emphasis.
4. **Write the source page** at `wiki/sources/<slug>.md` with full frontmatter, TL;DR, key claims, quotes, and wikilinks to every entity/concept/jurisdiction it touches.
5. **Update downstream pages.** For each wikilink in the source page:
   - If the target page exists: update it with new facts, citing the new source. Note contradictions explicitly.
   - If it doesn't: create a stub with frontmatter and whatever the new source gives you. Stubs are fine — they get filled in by future sources.
6. **Update `index.md`.** Add the source under Sources; add any new entity/concept/jurisdiction pages under their categories.
7. **Append to `log.md`.** Use the exact prefix format (see Logging).
8. **Report.** Tell Lucas: what you filed, which downstream pages you touched, any contradictions flagged, any stubs created, any open questions worth chasing.

A typical ingest touches 5–15 pages. That's expected.

### Query

When Lucas asks a question:

1. **Read `index.md` first** to locate relevant pages.
2. **Read the pages**, follow wikilinks as needed.
3. **Synthesize an answer** with inline `[[source-slug]]` citations.
4. **Offer to file the answer.** If the answer is non-trivial (comparison, thesis, analysis), ask whether to save it as a `wiki/syntheses/<slug>.md` or `wiki/comparisons/<slug>.md`. Good answers should compound, not vanish into chat.
5. **Log the query** if it produced a filed page.

### Bulk ingest (amendment 2026-04-20)

When ingesting many sources at once (hundreds of blog posts, help articles, a crawled site), switch to **bulk mode** — the standard per-source template explodes the wiki with duplicate stubs. Rules:

- **No new stubs.** Only link to entity/concept/jurisdiction pages that **already exist**. If a bulk source is substantively about a not-yet-covered topic, flag it in the phase report; Lucas decides whether to create the page before moving on.
- **Lighter source-page template.** Frontmatter + 1-paragraph TL;DR + 3–5 key claims + wikilinks to existing pages only. Skip the quotes, open-questions, and exhaustive entity-fanout sections.
- **Per-collection inventory synthesis.** For each bulk collection (e.g., a blog, a help center, a docs site), create one `wiki/syntheses/<collection>-inventory.md` that groups the source pages by topic. This gives the collection shape without needing a 300-item scroll through `index.md`.
- **Exceptions for stub creation:** ok to create a brand-new entity page for a major regulator (HMRC, CRA, ATO, BMF, etc.) or jurisdiction when a whole guide is about that body — these are infrastructure pages, not duplicative stubs.
- **Log once per phase, not per source.** A bulk run gets one log entry per phase with counts, coverage notes, and a link to the inventory synthesis.
- **Update `index.md` once per phase.** List the inventory synthesis under Syntheses with the phase's source-count; individual source pages don't need listing in `index.md` when an inventory synthesis covers them.
- **Be honest about heterogeneity.** Content-marketing listicles ("5 best X") should get one-sentence TL;DRs and be tagged low-signal in the inventory. Deep tax guides get full lighter-template treatment. Don't pretend every source is equally informative.

### Lint

Never auto-lint or auto-fix. Always report first, let Lucas approve each change.

When Lucas asks for a lint pass, check:
- Contradictions between pages that aren't flagged.
- Stale claims: entity/jurisdiction pages whose "current state" predates newer sources.
- Orphans: pages with no inbound wikilinks.
- Missing pages: concepts/entities referenced in text but lacking their own page.
- Broken wikilinks.
- Index drift: pages not in `index.md`, or entries in `index.md` whose page is gone.
- Gaps: important sub-topics where Lucas has no sources yet — suggest what to read.

Output a prioritized findings report. Do not touch files until Lucas greenlights specific fixes.

---

## Indexing (`index.md`)

Content-oriented. Organized by category (Sources, Entities, Concepts, Jurisdictions, Comparisons, Syntheses). Each entry: `- [[slug]] — one-line summary` (plus date for sources).

Update on every ingest and whenever a new page is created.

---

## Logging (`log.md`)

Append-only. Every entry starts with the exact prefix:

```
## [YYYY-MM-DD] <op> | <short title>
```

Where `<op>` is one of: `ingest`, `query`, `lint`, `schema`, `refactor`.

Body: 2–6 bullets — what happened, which pages were touched, anything notable. Keep it skimmable so `grep "^## \[" log.md | tail -20` gives a useful timeline.

---

## Domain guardrails (crypto tax specifics)

- **Jurisdictional precision.** A claim about "wash sale rules" means nothing without a jurisdiction. Tag every tax claim with the country/regime it applies to. Default to US if unstated but confirm with Lucas.
- **Time sensitivity.** Tax rules change. Every claim on an entity/concept/jurisdiction page should cite a dated source. When a newer source supersedes an older one, update the page and move the old claim to a `## Historical` section — don't silently drop it.
- **Competitor context.** Treat CoinLedger competitors (Koinly, CoinTracker, TokenTax, ZenLedger, TaxBit, Awaken, Crypto Tax Calculator) as first-class entities. Pricing, feature, and positioning changes are always worth filing.
- **Regulatory entities.** IRS, Treasury/FinCEN, SEC, CFTC, HMRC, CRA, ATO, ESMA, etc. — each gets an entity page.
- **Guidance hierarchy.** On US pages, distinguish statute → Treasury regulations → IRS Revenue Rulings/Notices → FAQ/guidance → court rulings. Don't flatten these.
- **Don't over-explain basics to Lucas.** He knows cost basis, HIFO/FIFO/Spec ID, staking/DeFi mechanics, 1099-DA, the broker rule saga. Frame at the level of a crypto tax practitioner, not a layperson.

---

## Tooling

- Wiki is a plain markdown directory. Works with Obsidian; wikilinks and frontmatter are Obsidian-compatible.
- Images under `raw/assets/` can be referenced with standard `![[image.png]]` or `![](raw/assets/image.png)`.
- No search engine yet. At this scale `index.md` is sufficient. Revisit if the wiki passes ~100 sources.
