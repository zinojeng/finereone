# inker_slope

- **Full citation**: Inker LA, Heerspink HJL, Tighiouart H, et al. A meta-analysis of GFR slope as a surrogate endpoint for kidney failure. Nat Med. 2023;29(7):1867-1876. DOI: 10.1038/s41591-023-02418-0. PMID: 37330614. PMCID: PMC13037386.

- **Source obtained**: FULL TEXT (retrieved via PubMed Central, PMC13037386; PDF download from EuropePMC was POLLUTED — wrong paper returned [Engineering Bacteria as Living Therapeutics in Cancer Therapy, Advanced Science 2025] — deleted immediately; full text confirmed via PMC XML read covering Introduction, Results, Discussion, Methods, and all Extended Data Tables)

- **Role in FIND-CKD**: Cited as FIND-CKD ref [21] to justify use of eGFR slope as a surrogate primary endpoint for kidney failure. FIND-CKD's trial team invoked this meta-analysis to argue that a treatment benefit on eGFR slope predicts a benefit on hard kidney endpoints (KFRT/doubling of serum creatinine), thereby making slope a valid primary endpoint. However, FIND-CKD used the *chronic slope* (post-3-month) rather than the 3-year *total slope* — a distinction that Inker 2023 itself flags as critical, since chronic slope is the *weaker* of the two surrogates evaluated. This discordance is the kernel of the primary-endpoint critique: citing Inker 2023 for chronic slope validity overstates what the paper actually demonstrates for that metric.

- **Key findings** (all numbers verified directly from full text):

  - **Population and scope**: Individual participant data meta-analysis; 66 RCT treatment comparisons spanning four disease groups — CKD from other/unspecified causes (28 studies), Diabetes (21 studies), Glomerular disease/GN (10 studies), Cardiovascular disease/CVD (7 studies); 17 distinct interventions; total N = 186,312 participants; median follow-up 35 months (IQR 22-52). Interventions included RASB, SGLT-2 inhibitors (4 trials), GLP-1 agonists, DPP-4 inhibitors, MRA, endothelin receptor antagonists, immunosuppression, blood-pressure and dietary interventions.

  - **Primary clinical endpoint**: Composite of KFRT (dialysis initiation or kidney transplant) + sustained eGFR <15 mL/min/1.73 m² + doubling of serum creatinine; 11,396 patients (6.1%) reached endpoint.

  - **3-year TOTAL slope (primary surrogate)**: Trial-level R² = 0.97 (95% BCI 0.82-1.00). Meta-regression slope = -0.35 (95% BCI -0.42 to -0.29) per mL/min/1.73 m²/year. A 0.75 mL/min/1.73 m²/year greater treatment benefit on total slope is associated with a 23.3% lower HR for the clinical endpoint (95% BCI 19.3%-27.2%). The 95% Bayesian prediction interval (BPI) for a large trial (N=1600) at this treatment effect definitively excludes HR ≥1: BPI 0.60-0.89. Intercept = -0.04 (95% BCI -0.09 to 0.01), consistent with no spurious benefit when slope is neutral.

  - **CHRONIC slope (post-3-month slope; the metric FIND-CKD used)**: Trial-level R² = 0.55 (95% BCI 0.25-0.77) — classified as only "moderate" surrogate performance. Meta-regression slope = -0.33 (95% BCI -0.46 to -0.20). The 95% BPI for the same 0.75 mL/min/1.73 m²/year treatment benefit does NOT exclude HR ≥1 even in a large trial: BPI 0.51-1.18. The threshold treatment effect on chronic slope required to achieve ≥97.5% probability of clinical benefit is 1.26 mL/min/1.73 m²/year — nearly 3-fold higher than the 0.44 mL/min/1.73 m²/year threshold for total slope.

  - **Diabetes subgroup** (most relevant to FIND-CKD population; 21 studies, verified from Extended Display Table 7): At a 0.75 mL/min/1.73 m²/year benefit on *chronic* slope, the predicted HR is 0.86 with 95% BPI 0.63-1.13 in a large trial (PPV 0.89) — does NOT definitively exclude HR ≥1. At the same effect size on *total* slope, HR is 0.75 (BPI 0.59-0.93), PPV 0.99 — definitively beneficial. Chronic slope treatment effect across 21 diabetes RCTs: +0.69 mL/min/1.73 m²/year (95% CI 0.37-1.00).

  - **CVD subgroup caution**: R² for chronic slope in CVD group = 0.47 (95% BCI 0.01-0.99), lowest across disease groups, with very wide BCI precluding firm conclusions.

- **How it SUPPORTS or CHALLENGES FIND-CKD's conclusions**:

  - **Supports**: Inker 2023 provides genuine mechanistic and statistical justification that eGFR slope is biologically plausible as a surrogate for kidney failure. Results are consistent across CKD severity (GFR above and below 60 mL/min/1.73 m²) and across albuminuria subgroups (ACR >30 mg/g). A meaningful positive chronic slope in the treated arm of FIND-CKD would, probabilistically, forecast some clinical benefit.

  - **Challenges**: Inker 2023 explicitly identifies chronic slope as the *weaker* of the two validated metrics, with R² of 0.55 vs 0.97 for total slope. The paper states: "the BPI are considerably wider for the chronic slope than the 3-year total slope." For a large RCT claiming benefit via a 0.75 mL/min/1.73 m²/year chronic slope improvement, a 95% BPI of 0.51-1.18 still includes HR ≥1 — meaning the clinical inference is uncertain. FIND-CKD citing this paper to validate its chronic-slope primary endpoint is selective: the paper's headline message is that *total slope*, not chronic slope, achieves strong surrogate validity. Additionally, Inker 2023 warns that acute GFR dips (negative acute effects) characteristic of some agents are captured in total slope but excluded from chronic slope; when a drug's mechanism involves an acute dip (e.g., SGLT-2 inhibitors, finerenone's hemodynamic effects), chronic slope may *overestimate* the true sustained benefit by stripping out the early component that contributes to the composite clinical endpoint. This is particularly pertinent if FIND-CKD's investigational agent causes an early GFR dip.

- **Limitations of this reference itself**:
  1. All surrogate validation rests on the same pool of completed RCTs; applications to trials with interventions substantially different from those in the pool carry added uncertainty explicitly acknowledged by the authors.
  2. Only interventions with negative or neutral acute effects on GFR predominate in the dataset; the authors caution that "applications to future trials with especially large acute effects may incur added uncertainty."
  3. The CVD subgroup (7 studies) is too small to generate reliable subgroup-specific surrogate estimates; wide BCIs prohibit firm subgroup conclusions.
  4. GFR is estimated from creatinine (CKD-EPI 2009); interventions affecting body composition or dietary protein intake (confounders of serum creatinine) may introduce non-GFR-related acute slope artifacts — cystatin C is recommended as a robustness check.
  5. Prediction intervals assume future trials resemble historical ones; a trial in a novel population or with an unprecedented magnitude of acute effect is extrapolating beyond the validation set.
  6. Follow-up time differences between studies (shorter in CVD) may confound cross-disease comparisons.
