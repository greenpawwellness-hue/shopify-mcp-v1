# Green Paw Wellness — Parasite Cleanse review: handoff brief

Paste this into a new chat to resume. Everything below is settled unless marked OPEN.

---

## Business context

- **Green Paw Wellness** — herbal supplements for dogs and cats, sold on Shopify (greenpawwellness.com).
- **Product under review:** Parasite Cleanse, a capsule containing **wormwood, black walnut, clove, pumpkin seed**.
- Current label dose: **1 capsule per 20 lb daily**, used in 14-day cycles.
- **The label lists every ingredient amount — nothing proprietary.**
- **Only one capsule size is available.** A second, smaller capsule is not an option.
- **All products in the line share the same directions block.** Product-specific *warnings* may be possible — unconfirmed.
- A label reprint takes about **two weeks**.
- Herbs sourced from **Herbco (Monterey Bay Herb Co.)** and **Nutriland Group**, plus one other supplier not yet identified. Herbco sells cut/sifted and powdered **raw herb only, no extracts** — their wormwood powder is **wild-crafted**.

## Field safety record

- Roughly **80+ cases**, **2 adverse events**, both gastrointestinal, both resolved on stopping, neither escalated to a vet.
- **Zero neurological events** — no tremors, ataxia or seizures. This is the thujone signature and it is absent.
- One event: an owner **split a capsule between two cats and both vomited**. Note this was at approximately the *correct* dose, and splitting means opening — loose bitter powder met oral mucosa that an intact capsule bypasses. Likely local irritation, not systemic toxicity.
- Other event: bad diarrhoea, owner stopped immediately.

## Key numbers already derived

**Thujone (from wormwood)**
- EMA accepts 3.0 mg/day for a 70 kg human, max 2 weeks = **0.043 mg/kg/day**.
- Per-capsule target: **~0.35 mg thujone**. At that level a 20 lb dog sits ~**285×** below the rodent BMDL₁₀ for clonic seizures (11 mg/kg/day), ~2,600× below the lowest seizure-producing dose (100 mg/kg), ~5,000× below the oral LD₅₀ (192 mg/kg).
- **Dried wormwood spans roughly 0.002%–1.0% thujone — a 500-fold range** across chemotypes and origins (oil yield 0.2–1.5%; thujone 1–65% of that oil; six-plus European chemotypes, several essentially thujone-free). **Herb weight therefore does not specify a dose.** Wild-crafted sourcing makes batch variation the expected behaviour.
- Thujone half-life is short (≤3.55 h in rats) so it does not accumulate; P450 hydroxylation is a *detoxification* step yielding metabolites less potent than the parent.

**Eugenol (from clove)**
- WHO ADI **2.5 mg/kg bw/day**. Clove bud is ~10–15% eugenol; use 15% when setting ceilings.
- **Confirmed: 75 mg clove per capsule = 11.25 mg eugenol.**
- Dogs: **1.24 mg/kg/day** — half the ADI. No issue.
- 10 lb cat on one capsule daily: **2.48 mg/kg/day** — at the ADI.
- 8 lb cat: **3.10 mg/kg/day** — 1.24× over.
- Margin to observed hepatotoxicity (400 mg/kg in glutathione-depleted mice, the closest model of a cat): **81–161×**.
- Cats are UGT-deficient *and* glutathione-limited, so eugenol's primary clearance route is impaired. **Thujone is much less of a feline problem** — its rate-limiting step is P450 hydroxylation, which cats have; glucuronidation only acts later on already-weakened metabolites.
- **If reformulating: 40 mg clove** puts every cat from 6 lb up under the WHO ADI. (15 mg carries a full 10× cat factor but is a bigger change than needed.)

## Decisions made

1. **Clove stays at 75 mg this cycle.** Revisit at the next natural reformulation, target 40 mg. This is a deliberate, reasoned decision — not an oversight.
2. **Gates: under 8 lb and under 6 months → see your veterinarian.** These must go on the **label**, not only the website — on this path they are the safety control, not a caution.
3. **Daily dosing preserved.** Anthelmintic efficacy is time-dependent: albendazole cure rates rise from 40%→83% (*T. trichiura*) and 54%→93% (hookworm) going from one dose to three consecutive days. An every-other-day schedule was proposed and **withdrawn** for this reason.
4. **Whole capsules only — never opened or split.** Splitting caused the one cat incident and cannot be measured. Do **not** tell cat owners to give half a capsule.
5. **Hard cap of 4 capsules/day** regardless of weight (linear dosing over-shoots metabolic scaling above ~80 lb).
6. **14 days on, minimum 14 days off**, wording made unambiguous. Rest-phase product sold for the off period.
7. **No binders during the cycle** — activated charcoal, bentonite, zeolite adsorb the actives in the gut. Binders belong in the rest phase. (Their Detox Bundle does **not** contain charcoal — confirmed, that finding is closed.)
8. **Claims cleanup** across the site — see below.

## Regulatory framework

- **There is no DSHEA for animal products.** Structure/function claims legal on a human supplement ("supports gut health") are **drug claims** for animals. CPG 690.100 was **withdrawn 20 Feb 2020**.
- FDA has cited near-identical language to their copy: *"paralyzes the tapeworms forcing them to release themselves from the digestive tract."*
- FTC requires "competent and reliable scientific evidence" for efficacy claims; testimonials carry the same claim as if the brand made it.
- **Safe territory:** composition, nutritive value, traditional use framed as history, quality and testing process.
- **Product name:** "dewormer" must go everywhere. "Parasite Cleanse" is a lower order of risk — an attorney question, not urgent.

## Factual correction to make

**Cucurbitin** is the non-protein amino acid (3-amino-pyrrolidine-3-carboxylic acid) in pumpkin seed. **Cucurbitacin B** is a triterpenoid — a different molecule. Current copy calls cucurbitacin an amino acid, merging the two.

## STILL OPEN

- Milligrams of **wormwood, black walnut, pumpkin seed** per capsule (readable off their own label).
- **GC-MS thujone assay** on current lot — ideally three lots, to see how much supply varies.
- **Milled herb vs dry extract** for anything not from Herbco. Ask for *ratio and carrier*, not whether it's liquid — dry extracts are powders and look identical in a capsule.
- **How many of the ~80 cases were cats?** One in forty is noise; one in five is a signal.
- **Cycles per year** number for the label (4 is a defensible default).
- Whether **any other product in the line contains clove**, and whether a daily supplement carries cycle language meant only for the cleanse.
- **SEO title field** — indexed title reads "Dewormer for Dogs | Natural Parasite Cleanse Supplement". Shopify → Products → Search engine listing.
- Whether **warnings can be product-specific** on their shared label format.
- **Mycotoxin screening** on the black walnut (moldy hulls, not the botanical, are the canine concern).

## Working documents

Committed to **`greenpawwellness-hue/shopify-mcp-v1`**, branch **`claude/parasite-formula-review-rv2lqi`**:
- `docs/parasite-formula-review.html` — full formulation and toxicology review
- `docs/website-change-list.html` — page-by-page copy edits with paste-ready blocks
- `docs/HANDOFF.md` — this file

Published artifacts:
- Review: https://claude.ai/code/artifact/c5523ec5-c5b7-4c84-a3db-1fc91550bef9
- Change list: https://claude.ai/code/artifact/5f580a32-e13e-4f41-b5b3-2f3b426b7d72

## Note for the assistant picking this up

greenpawwellness.com was **blocked by the network egress policy** in the previous session, so all quoted site copy is reconstructed from search-engine indexing and has **not** been verified against live pages. If you can reach the site, read it and audit properly. Otherwise ask the user to paste the product page, both blog posts, label text and email copy.

Useful technique the user has been given: `site:greenpawwellness.com "phrase"` in Google finds every indexed page containing a phrase, including blog bodies and meta fields that Shopify's admin search misses.

Tone note: the user is conscientious and was anxious through much of the prior session. They caught two things the assistant missed — the systematic capsule-rounding error and the charcoal interaction — and correctly rejected a proposed every-other-day schedule that would have degraded efficacy. Give them straight numbers with honest margins, flag when a figure is derived judgement rather than a published limit, and don't escalate past what the evidence supports.
