# Submission notes — *Titrating Against the Wrong Metric*

> **Rewritten 2026-07-17** after the four-auditor resolution round. **This file supersedes the previous version**, which described a superseded 22-reference draft (different title, no figures) and an extraction run that supplied empty must-fix/discuss lists. That run's headline risk — "Vibhatavata/Turcu 2026 is not cited anywhere" — **is resolved**: it is now ref 1, the manuscript positions explicitly against it (§2), and §8 engages its inferences directly.
>
> **Files:** `manuscript.md` (audit-annotated: carries the `<!-- src: -->` grep trail, Evidence-discipline note, and Editorial changelog) · `manuscript_clean.md` (**submission-clean**: src comments stripped, pipeline apparatus removed — verified 0 hits for `<!-- src:`) · this file.

---

## 1. Target journal, and why

**Primary target: *Hypertension* (American Heart Association), category Review.**

The case for it:

- **The conversation is already there.** Ref 1 (Vibhatavata & Turcu, *Hypertension* 2026;83(5):e26229) and ref 11 (Li 2026, *Hypertension* 83(5):e26048) are both in this journal, **in the same issue**. This manuscript is an explicit extension of ref 1 and its flagship dataset is ref 11. Placing it elsewhere separates the argument from the two papers it is in dialogue with.
- **The audience is the right one.** The deliverable (§10, Table 3) is a trial specification. *Hypertension* readers design and run these trials.
- **Length tolerance.** AHA Reviews accommodate a longer main text than the endocrine alternatives — relevant given the current overrun (§3).

The case against, equally honestly:

- ***Hypertension* Reviews are frequently invited.** An uninvited Review may be desk-rejected on category grounds regardless of merit. **A presubmission enquiry is strongly recommended before any formatting investment.**
- **The likely referees are the people being engaged.** A.F. Turcu and/or A. Vaidya author refs 1, 3, 5 and 22. §2 credits ref 1 explicitly and at length; §8 argues *against* one of its inferences using its own data. Defensible, and we think correct — but not a low-risk referee draw. See §7.

**Fallback ladder, in order:**

| # | Journal | Main-text budget | Notes |
|---|---|---|---|
| 1 | *Journal of Hypertension* (ESH) | ~4,000 | Requires the deeper trim (§7 into Table 2 entirely; merge §5 into §4). British spelling acceptable. |
| 2 | *European Journal of Endocrinology* | ~5,000 | Publishes ref 13 (Uslar) and ref 27 (SPAIN-ALDO); endocrine readership familiar with PAMO. |
| 3 | *Hypertension Research* (JSH) | ~5,000 | **Caution: Yoshida & Shibata publish the competing reviews here (ref 6), and ref 6 is our highest overlap risk.** Submitting here likely routes the manuscript to the one referee whose own review most overlaps it. |
| 4 | *J Clin Endocrinol Metab* | ~6,000 | Publishes refs 2 and 26 (the guideline and its systematic review). Most tolerant of the current length. |

*All limits above are estimates, not verified against current Instructions for Authors. See §2.*

---

## 2. Format compliance checklist

**⚠️ Every limit below is an ASSUMPTION until checked against the current Instructions for Authors.** Journal author guidelines are not in the local corpus, and this project's evidence rules forbid asserting values that cannot be verified. Check these first — they determine how much trimming is real work.

| Item | Current state (measured 2026-07-17) | Assumed limit | Status |
|---|---|---|---|
| **Main text (§1–§11)** | **≈6,924 words** | 5,000 *(unconfirmed)* | ❌ **OVER by ≈1,920.** Trim plan in the manuscript's word-count block and §3 below. |
| **Abstract** | **258 words**, structured (Background / Objective / Findings / Conclusions) | 250, structured | ◐ **Over by 8.** Trivial cut. **Also confirm the required section headings** — ours are non-standard ("Findings" rather than "Methods/Results"), appropriate for a Review but must be checked against the category template. |
| **References** | **31** | No fixed AHA limit for Reviews | ✓ Verified this round: **true first-citation order**, all 31 cited, none orphaned, none missing (checked programmatically post-edit). |
| **Figures** | 3 | — | ⚠️ **Figures 1 and 3 are Mermaid source; Figure 2 is a plotting specification.** Journals accept none of these. Export to vector (SVG/EPS) at ≥1200 dpi equivalent. |
| **Tables** | 3 | — | Table 3 is the designated first item to move to a Data Supplement. |
| **Display items total** | 6 | often ~6–8 | ✓ |
| **Running head** | 48 characters incl. spaces | ≤50 | ✓ |
| **Spelling** | US English, AHA house style (`mm Hg`, `-ize`, `hypokalemia`) | — | ✓ for AHA. British spelling acceptable on fallbacks 1–2; no pass needed. |
| **Nonstandard abbreviations table** | Present | AHA requirement | ✓ |
| **Citation numerals** | Bracketed `[n]` in source | AHA wants superscript | Apply at typesetting. |

**Already stripped from `manuscript_clean.md`** (verified by grep, 0 hits each): all `<!-- src: -->` comments, the pre-submission action block, the alternative-titles block, the Evidence-discipline note, the Editorial changelog, and the word-count trim-guidance block. **Re-verify after any hand edit.**

**One decision left open:** the reference list carries no evidence-discipline annotations (those live in the Evidence-discipline note, which is deleted from the clean copy). If you want the abstract-only status of refs 4, 11, 22 and 23 visible to the editor, it is currently disclosed **in the text** (§5 and §9, in the manuscript's own voice) rather than in the reference list. We think that is the right place for it.

---

## 3. The length problem — read before trimming

The audit round **added ≈1,600 words** to the main text. That was not padding; it was the cost of making the manuscript defensible:

- **§5's Hu-parity counter-argument** — the strongest published objection to the central thesis, previously sitting unstated in a Table 1 cell
- **§7's rewritten Exhibit 3** — the prior version's "ranking inversion" was an artifact of comparing office BP against ambulatory BP, i.e. the exact error the review condemns
- **§6's spironolactone-arm office:ambulatory ratio** (2.19 vs finerenone's 1.79) — reported because it *disciplines* our own argument
- **§10(i)'s reworked warrant** — renin demoted from sole primary endpoint to co-primary

**Do not trim any of these to hit a word count.** Removing them reintroduces the precise errors this round fixed, and each is the kind of thing a hostile referee finds first. Cut instead from §4, §9, §10 and Table 3 — all largely prose restatements of material that already exists in tables. The ordered trim plan (≈1,700 words recoverable, reaching ≈5,130) is in the manuscript's word-count declaration block.

---

## 4. Novelty statement / cover-letter angle

**The one-sentence claim:**
> Every recent review asserts that renin matters in primary aldosteronism; this one measures how far the field's metrics disagree with each other, and shows that one of the comparisons the field is implicitly making cannot presently be made at all.

| | |
|---|---|
| **Not ours** | The qualitative thesis — BP lowering dissociates from adequate MR blockade; milligram equivalence is not potency equivalence — is **Vibhatavata & Turcu's** (ref 1). §2 says so explicitly. **Do not let the cover letter blur this; the likely referee wrote it.** |
| **Ours (i)** | **The PAMO juxtaposition.** Ref 1 cites the finerenone cohort but reports only its BP and renin figures. Placing 29.1%/20.0% beside PAMO's 52.9%/18.3% renders the dissociation numerical. |
| **Ours (ii)** | **The office-to-ambulatory inflation factor quantified** (≈2.3×), in both arms of the only two-arm dataset — converting ref 1's qualitative "the office declines are larger" into a falsifiable measurement. |
| **Ours (iii)** | **The demonstration that no cross-class BP-versus-renin ranking is currently constructible** in PA, because no two studies share both a measurement modality and a class contrast. A negative result about the evidence base. |
| **Ours (iv)** | **The 11-DOC asymmetry argument** — renin is not a common currency across receptor blockade and synthesis inhibition — which runs *against* ref 1's own inference using that review's own data. Most original, most contestable. |
| **Ours (v)** | **The deliverable:** a measurement specification for the head-to-head trial everyone demands (§10, Table 3). Everyone calls for the trial; nobody has specified what it must measure. |

**Tone guidance:** lead with (v) and (iii), not (iv). Exhibit 4 is the most interesting argument in the paper and the most likely to draw a fight from the referee it engages. Let it be discovered in the manuscript rather than advertised in the letter.

---

## 5. Suggested cover letter (draft — fill placeholders)

> **[PLACEHOLDER — letterhead / date]**
>
> Dear Dr [PLACEHOLDER — Editor name],
>
> We submit for consideration as a Review, *"Titrating Against the Wrong Metric: Blood Pressure, Renin, and the Measurement of Treatment Adequacy in Primary Aldosteronism."*
>
> There is broad agreement that renin de-suppression, not blood pressure normalization, marks adequate mineralocorticoid receptor blockade in primary aldosteronism. The 2025 Endocrine Society guideline codifies it; the PAMO consensus operationalizes it; recent reviews in this journal restate it. What no one has done is ask how far the available metrics actually disagree with one another — or whether renin means the same thing under receptor blockade as under synthesis inhibition.
>
> This review audits the metrics rather than asserting one. Applying the field's own consensus instrument to its newest data, finerenone in primary aldosteronism reproduces conventional clinical response almost exactly (20.0% vs 18.3%) while delivering roughly half the biochemical response (29.1% vs 52.9%). Concurrently measured office systolic blood pressure reads approximately 2.3 times daytime ambulatory in the same cohort — and office blood pressure is what clinicians titrate against, and what the ongoing trials titrate against. Tabulating renin yield per class then produces a negative result we consider the manuscript's most useful contribution: because published blood pressure effects in this disease are reported in at least three non-interchangeable modalities, and no two studies share both a modality and a drug-class contrast, no cross-class blood-pressure-versus-renin ranking can presently be constructed at all. Finally, we argue that 11-deoxycorticosterone accumulation upstream of synthase blockade means aldosterone synthase inhibitor and mineralocorticoid receptor antagonist arms matched on renin are not thereby matched on receptor activation — an argument that runs against the inference drawn in Vibhatavata and Turcu's recent review in this journal, and which we make using that review's own data.
>
> We wish to be explicit about priority. The qualitative thesis — that blood pressure lowering dissociates from adequate receptor blockade, and that milligram equivalence is not potency equivalence — is Vibhatavata and Turcu's, and Section 2 credits it as theirs. This manuscript is an explicit extension of that review, not a competitor to it. What we add is measurement, a self-audit of our own exhibits (Section 9), and a specification for what the randomized head-to-head trial the field keeps calling for must actually measure (Section 10, Table 3).
>
> The manuscript makes no new empirical claim. Every value is drawn from a published report and carries the epistemic status its source permits; where sources were available to us only as structured abstracts, we say so in the text and assert nothing held behind the paywall.
>
> The manuscript is not under consideration elsewhere, and all authors have approved the submission. [PLACEHOLDER — confirm; add any required statements on prior presentation or preprint deposition.]
>
> Yours sincerely,
> **[PLACEHOLDER — corresponding author, degrees, affiliation, contact]**

**For a presubmission enquiry instead** (recommended for *Hypertension*), cut to: paragraph 1, the first three sentences of paragraph 3, and the priority paragraph. Ask directly whether an uninvited Review in this space would be considered.

---

## 6. Placeholders the author MUST fill

None of the following was assigned, received, or is knowable by the drafting process. **Do not submit any of these unedited.**

- [ ] **Authors** — names, degrees, ORCIDs, affiliations, order. *(The drafting process assigned no authorship. Do not invent authors.)*
- [ ] **Corresponding author** — name, department, full postal address, telephone, email.
- [ ] **Subject terms (AHA)** — suggested: Hypertension; Endocrinology; Pharmacology; Clinical Studies. Select at submission.
- [ ] **Acknowledgements** — each named individual must give written permission.
- [ ] **Sources of Funding** — explicit "no specific funding" statement, or all grant numbers + bodies.
- [ ] **Disclosures / COI** — **critical; see below.**
- [ ] **AI-Use Disclosure** — suggested text is in the manuscript; **check against the target journal's current policy.** AHA, ICMJE and Elsevier differ in wording *and* required placement. Do not omit.
- [ ] **Author Contributions (CRediT)**.
- [ ] **Ethics/IRB** — not applicable (no human subjects, no new data); state so if the form demands it.
- [ ] **Keywords** — 8 supplied; trim if the journal caps at 6.

**On COI — this is not a formality.** The manuscript adjudicates between the products of **Bayer** (finerenone), **Daiichi-Sankyo** (esaxerenone), **AstraZeneca/CinCor** (baxdrostat), **Damian Pharma** (dexfadrostat) and **Recordati** (osilodrostat). Each author must individually declare **or explicitly negate**, *for each company named*: honoraria; advisory board membership; speakers' bureau; research funding (institutional or personal); travel support; consultancy; stock or equity. A thin disclosure on a paper of this kind is a credibility problem independent of the science.

*(The manuscript records, in Disclosures, that ref 1's corresponding author discloses an AstraZeneca advisory role and a local-PI role on an AstraZeneca trial. This is stated because §2 and §8 engage that review's inferences directly and readers are entitled to weigh both parties' interests — not as an insinuation, and it does not substitute for our own disclosure.)*

---

## 7. Honest open risks

Ordered by how much damage each would do.

1. **Duplication / priority risk versus ref 6 (Yoshida & Shibata 2026, *Hypertens Res*) — the highest risk in the set.** Its abstract already couples PAMO, post-treatment renin as a response marker, finerenone, esaxerenone and ASIs in PA — this manuscript's exact axis — and **we hold it at abstract level only**. If its full text performs the PAMO juxtaposition or raises the 11-DOC asymmetry, Exhibits 1 and 4 lose their novelty claim. **Action: retrieve and grep-check the full text for "PAMO", "11-DOC", "ambulatory", "52.9"/"29.1" BEFORE any presubmission enquiry asserts priority.** Compounding hazard: fallback journal #3 is where Yoshida/Shibata publish.
2. **Four further 2026 reviews unread in full text** (Rossi, *Nat Rev Endocrinol*; Lu, *Eur J Pharmacol*; Elton-Bott, *Hypertension*; Menino, *Endocrine*). Same check required. §2's novelty claim is now scoped to "the reviews we were able to read in full text" — honest, but a referee holding one of these four can still puncture it.
3. **Ref 1's unresolved "[11]".** Ref 1 cites an unidentified reference 11 for "the proportions achieving reversal of renin suppression with MRAs" — a live candidate for the PAMO paper. Our local copy's reference list is **truncated at 8 of 83**, so we cannot check. If [11] *is* PAMO, §2's and §5's framing ("that review does not report PAMO response categories for the finerenone cohort") remains literally true but is rhetorically much weaker. **Resolve from the Europe PMC PDF before submission.**
4. **Referee draw.** The likely referees author refs 1, 3, 5 and 22. §8 argues against ref 1's inference on baxdrostat's 11-DOC. The argument is careful, uses their own data, is framed as interpretability rather than refutation, and §2 credits their priority generously — but it remains a paper that tells its most likely referee they drew the wrong inference.
5. **Abstract-only dependencies on load-bearing sources.** Exhibit 1 — the flagship — rests on **two abstract-only sources** (refs 4 and 11). We assert the response percentages (printed in the abstracts) but **not** the PAMO threshold definitions, which sit in paywalled tables. **We therefore cannot verify that the two datasets operationalized the PAMO criteria identically.** If they did not, Exhibit 1 weakens considerably. Stated in §5 and §9 in the manuscript's own voice rather than buried here. Also exposed: ref 22 (SPARK — figures transcribed from the trial's open-access ENDO 2025 abstract, not the paywalled NEJM letter) and ref 20 (Kishimoto). Obtain full texts for refs 4, 11, 20 and 22 before submission if at all possible. *(Ref 26's OUP 12-month free window may open ~2026-08-07 — worth one retry.)*
6. **Exhibit 3 is a negative result.** After the audit correction, §7 no longer delivers a positive finding; it demonstrates that a comparison cannot be made. We think this is more honest and more useful than the artifact it replaced, but a referee may read it as a section that does not earn its length. The trim plan compresses it into Table 2 if needed.
7. **The single-arm flagship is small and short.** N=57, 12 weeks, no comparator, enriched for eGFR ≥60. Every finerenone-in-PA dataset is ≤12 weeks with N≤60. SPARK's renin rose progressively to week 72, so a 12-week snapshot may mislead in either direction.
8. **ASI evidence is weak and we rely on it.** SPARK is open-label, single-arm, N=15, per-dose arms of n=2–7, no disease subtyping — the last publicly criticized in a *NEJM* letter (ref 29).
9. **The framework itself is interventionally unvalidated.** It remains unproven that escalating an MRA to raise renin *after* BP control improves hard outcomes. The guideline rates the relevant recommendation conditional, very-low-certainty (2 | ⊕OOO). The manuscript audits the metrics; it does not validate them — and §10(i) was reworked this round specifically so it does not nominate an unvalidated biomarker as a definitive trial's sole primary endpoint.
10. **Word count.** ≈1,920 over the assumed limit; the limit itself is unconfirmed.
11. **Fast-moving field.** FAIRY (NCT06457074), BaxPA and RETAME-PA (NCT06108427) are all live. A results readout during peer review could date §10 or force revision. Submit promptly; re-run a literature check at revision.
12. **Page ranges for refs 19 and 20 rest on external PubMed metadata**, not on local files (both local copies are abstract-only and contain no page range). Resolved in the manuscript's bibliographic resolution record naming PubMed as the authority and 2026-07-17 as the retrieval date; the inventory has been reconciled to match. Confirm against the publisher record if a copyeditor queries.

---

## 8. Pre-submission action list (short form)

- [ ] Confirm *Hypertension* Review word limit + abstract format/headings against current Instructions for Authors
- [ ] Send presubmission enquiry (Reviews are frequently invited)
- [ ] Retrieve ref 6 full text + the four abstract-level 2026 reviews; grep-check for overlap **(highest priority)**
- [ ] Resolve ref 1's "[11]" from the Europe PMC PDF
- [ ] Trim main text per the plan in the word-count block — do **not** cut §5's counter-argument, §6's two-arm ratio, §7's correction, or §9
- [ ] Cut abstract by 8 words
- [ ] Export Figures 1 and 3 from Mermaid to SVG/EPS; produce Figure 2 from its plotting spec
- [ ] Fill every placeholder in §6 — especially the per-company COI declarations
- [ ] Confirm `manuscript_clean.md` still greps 0 for `<!-- src:` after any hand edit
- [ ] Retry ref 26 full text after ~2026-08-07 (OUP free window)
