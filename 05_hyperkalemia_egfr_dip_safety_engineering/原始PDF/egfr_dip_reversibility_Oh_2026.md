---
title: "Causal Effects of Renin-Angiotensin-Aldosterone System Inhibition on Renal Function in Patients With Chronic Kidney Disease: A Quasi-Experimental Study"
authors: "Tae Ryom Oh, Jiyong Park, Hong Sang Choi, Harin Rhee, Gaeun Kang"
year: 2026
journal: "Clinical and Translational Science"
volume: "19:e70533"
doi: "10.1111/cts.70533"
pmid: "41876398"
source: "Europe PMC (Open Access, CC BY-NC)"
correspondence: "Gaeun Kang (gekang@jnu.ac.kr)"
received: "2025-10-13"
revised: "2026-02-14"
accepted: "2026-03-11"
---

# Causal Effects of Renin-Angiotensin-Aldosterone System Inhibition on Renal Function in Patients With Chronic Kidney Disease: A Quasi-Experimental Study

**Authors:** Tae Ryom Oh (1), Jiyong Park (2), Hong Sang Choi (3,4), Harin Rhee (5,6), Gaeun Kang (7,8)

**Affiliations:**
1. Department of Internal Medicine, Mokpo Hankook Hospital, Mokpo, Korea
2. Department of Management Information Systems, Terry College of Business, University of Georgia, Athens, Georgia, USA
3. Department of Internal Medicine, Chonnam National University Medical School, Gwangju, Korea
4. Department of Internal Medicine, Chonnam National University Hospital, Gwangju, Korea
5. Department of Internal Medicine, Pusan National University School of Medicine, Yangsan, Korea
6. Biomedical Research Institute, Pusan National University Hospital, Busan, Korea
7. Department of Pharmacology, Chonnam National University Medical School, Hwasun, Korea
8. Division of Clinical Pharmacology, Chonnam National University Hospital, Gwangju, Korea

**Keywords:** angiotensin receptor blocker; causal inference; causality; chronic kidney disease; estimated glomerular filtration rate; proteinuria; RAAS

---

## Abstract

Renin-angiotensin-aldosterone system inhibitors are widely prescribed for chronic kidney disease, but their causal effect on kidney function remains uncertain. This study investigated the impact of starting renin-angiotensin blockade on renal function in adults with kidney disease. A retrospective cohort study was conducted in Korea using a quasi-experimental staggered difference-in-differences design with propensity score matching to estimate time-varying treatment effects. Overall, 1,204 adults (375 treated and 829 contemporaneous not-yet-treated controls) were followed for 3 years. Initiation of angiotensin-converting enzyme inhibitors or angiotensin II receptor blockers was recorded, and treatment exposure was categorized monthly. The primary outcome was a change in estimated glomerular filtration rate after initiation, evaluated over sequential intervals up to 12 months. The overall average treatment effect of two-way fixed effects model was not statistically significant (-1.47 mL/min/1.73 m², p = 0.33). However, initiation was associated with an immediate and significant decline in eGFR at event time 0 (estimate: -3.87 mL/min/1.73 m², p < 0.05) and at event time 1 and 3 (p < 0.05). Beyond these early intervals, there was no evidence of progressive deterioration in kidney function during the 1-year follow-up. Declines following initiation of renin-angiotensin blockade are early, transient, and primarily hemodynamic in nature rather than reflective of structural kidney injury. Importantly, this quasi-experimental analysis of real-world data reproduced the findings of randomized trials, reinforcing current guideline recommendations to continue therapy in chronic kidney disease provided that reduction in filtration rate remains below the accepted threshold of 30%.

---

## Study Highlights

**What is the current knowledge on the topic?**
- RAAS inhibitors are guideline-recommended for CKD, yet an early decline in eGFR after initiation frequently prompts premature discontinuation.
- Whether this decline is transient or indicative of progressive renal injury has not been rigorously established from causal, real-world data.

**What question did this study address?**
- Does initiation of RAAS inhibition causally affect kidney function in patients with CKD?

**What does this study add to our knowledge?**
- Using a staggered difference-in-differences design with propensity score matching on real-world EMR data, the authors demonstrate that RAAS inhibitor initiation causes a statistically significant but transient eGFR reduction confined to the first 3 months, without progressive deterioration over 12 months.
- Declines were more pronounced and sustained in patients with high-grade proteinuria and were modest yet significant in those with advanced CKD.

**How might this change clinical pharmacology or translational science?**
- This quasi-experimental analysis of real-world data reproduced the findings of RCTs, validating the trial-emulation approach as a causal inference tool.
- Provides evidence that early eGFR declines within the KDIGO-recommended threshold (< 30%) do not predict subsequent renal deterioration, reinforcing guideline recommendations and discouraging premature RAAS inhibitor discontinuation.

---

## 1. Introduction

Chronic kidney disease (CKD) is a growing global health challenge, related to increased mortality, greater socioeconomic burden, and rising prevalence. Inhibition of the renin-angiotensin-aldosterone system (RAAS)—primarily through ACEi or ARBs—remains a cornerstone of therapy. RAAS inhibition is strongly recommended to slow progression to ESRD, reduce proteinuria, and mitigate cardiovascular risk.

Despite established benefits, the causal effect of RAAS inhibitors on renal function (eGFR) remains unclear across diverse populations and settings. Individual trials have reported heterogeneous effects on eGFR. Although meta-analyses reveal an initial eGFR decline following RAAS blockade, high-quality causal evidence linking RAAS inhibitors to long-term renal outcomes in real-world practice remains limited. This gap reflects the dynamic, time-dependent nature of eGFR, influenced by treatment exposure and disease progression.

RAAS blockade commonly induces a predictable and manageable decline in eGFR, but this reduction may raise concerns regarding treatment continuation. Therapy is often discontinued even when the eGFR decline remains within guideline-recommended thresholds, potentially resulting in adverse outcomes. Quantifying the dynamic causal effects of RAAS inhibitors on eGFR over time is crucial to inform clinical decision-making.

RCTs have demonstrated the efficacy of RAAS blockade in slowing CKD progression, but their external validity is constrained by strict eligibility criteria and prespecified outcomes. Real-world data from EMRs provide a valuable resource for evaluating treatment effects. In this study, a quasi-experimental approach was employed to emulate RCTs using observational data, aiming to isolate the causal effect of RAAS blockade on eGFR trajectories.

---

## 2. Methods

### 2.1 Study Population

EMR data were retrospectively extracted from Chonnam National University Hospital and Pusan National University Hospital. To ensure established CKD and exclude transient eGFR decline (e.g., acute kidney injury), enrollment required both diagnostic codes and longitudinal laboratory confirmation: patients had to have at least 10 serum creatinine measurements over a follow-up period exceeding 3 years. Cohort entry was defined independently of RAAS inhibitor initiation. Patients were not excluded based on events occurring after treatment initiation (such as AKI or treatment discontinuation).

Based on KDIGO guidelines, advanced CKD was defined as eGFR < 30 mL/min/1.73 m² (stages 4-5), and high-grade proteinuria as urine dipstick proteinuria ≥ 2+.

Control patients were selected from this same CKD-confirmed cohort and consisted of individuals who did not initiate RAAS inhibitor therapy during the predefined observation window.

Exclusion criteria included age < 19 years, pregnancy, dialysis, kidney transplantation, and hospitalization within 1 month prior to enrollment.

### 2.2 Data Construction

eGFR was calculated using the CKD-EPI equation. The calculated eGFR was maintained in its standard BSA-indexed form (mL/min/1.73 m²) without de-indexing for actual BSA. To standardize irregular testing intervals, data were aggregated monthly. Multiple values per month were averaged, and missing months were imputed using last observation carried forward. Patients were classified according to RAAS inhibitor use (treatment vs. control) and restructured into monthly longitudinal datasets.

### 2.3 Statistical Analysis

A quasi-experimental difference-in-differences (DID) design was employed. A two-way fixed effects (TWFE) model was applied to estimate the average treatment effect. A staggered DID model was employed, as patients in the treatment group received RAAS inhibitors at different times. The control group consists of "not-yet-treated" patients rather than a permanently untreated population. The "did" package in R, developed by Callaway and Sant'Anna, was used.

Propensity score matching (PSM) was employed to create a more comparable analytic sample. A nearest-neighbor 1:1 matching algorithm without replacement was applied, incorporating variables such as age, sex, BUN, serum creatinine, serum glucose, diabetes mellitus, and hypertension. Covariate balance after PSM showed all absolute standardized mean differences below the 0.1 threshold.

Subgroup analyses based on proteinuria status and advanced CKD were performed (full sample without additional PSM to preserve statistical power within each subgroup).

### 2.4 Informed Consent and Ethics

Conducted following the Declaration of Helsinki. Approval from IRBs of Chonnam National University Hospital (IRB No. CNUH-2024-147) and Pusan National University Hospital (IRB No. 2406-006-140). Requirement for informed consent was waived by the IRBs.

---

## 3. Results

### 3.1 Baseline Characteristics of the Study Population

Baseline characteristics compared control (n = 829) and treatment (n = 375) groups. Mean ages were similar (61 vs. 59 years, p = 0.43). Most laboratory parameters were comparable except for BUN, creatinine, potassium, and prevalence of hypertension and diabetes. The distribution of actual BSA was comparable (average BSA ~1.70-1.75 m²).

Statistically significant differences were observed in:
- Diabetes mellitus: control 354 (42.7%) vs. treatment 188 (50.1%), p = 0.019
- Hypertension: control 402 (48.5%) vs. treatment 214 (57.1%), p = 0.007
- Serum potassium: control 4.5 ± 0.7 vs. treatment 4.7 ± 0.7, p < 0.001

Missingness ranged from 18.6% to 76.5%.

### 3.2 Causal Effect of RAAS Inhibitors on Renal Function

The TWFE DID model showed no significant baseline effect. The estimated average treatment effect was -1.47 mL/min/1.73 m² (SE 1.42; p = 0.33), statistically nonsignificant.

Staggered DID model showed RAAS inhibitors exerted a statistically significant influence during the early post-treatment phase (0, 1, and 3 months). RAAS inhibitor therapy was related to eGFR reductions of -3.87, -2.34, and -2.54 mL/min/1.73 m² at event times 0, 1, and 3, respectively (p < 0.05 for all). These declines reflect the acute physiological effect of RAAS inhibition. This effect attenuated and became nonsignificant after 3 months. When aggregated across all post-treatment periods, the overall estimate was -1.02 (95% CB: -2.93 to 0.89), no statistically significant effect at the 5% level.

**Table 1 — Time-varying treatment effects estimated using staggered difference-in-difference models**

| Event time (months) | Estimate (mL/min/1.73 m²) | Std. error | 95% CI |
|---|---|---|---|
| -12 | 0.65 | 0.71 | -1.38 to 2.68 |
| -11 | 0.56 | 0.59 | -1.13 to 2.24 |
| -10 | 0.18 | 0.36 | -0.83 to 1.20 |
| -9 | -0.34 | 0.53 | -1.83 to 1.16 |
| -8 | -0.19 | 0.33 | -1.13 to 0.76 |
| -7 | 0.35 | 0.47 | -0.98 to 1.68 |
| -6 | -0.39 | 0.51 | -1.84 to 1.06 |
| -5 | 0.07 | 0.43 | -1.16 to 1.29 |
| -4 | -0.63 | 0.41 | -1.79 to 0.53 |
| -3 | -0.01 | 0.36 | -1.03 to 1.01 |
| -2 | -1.19 | 0.45 | -2.48 to 0.10 |
| -1 | -0.02 | 0.37 | -1.08 to 1.03 |
| **0** | **-3.87** | **0.80** | **-6.14 to -1.59** |
| **1** | **-2.34** | **0.74** | **-4.45 to -0.22** |
| 2 | -2.26 | 0.84 | -4.64 to 0.13 |
| **3** | **-2.54** | **0.85** | **-4.97 to -0.11** |
| 4 | -1.38 | 0.93 | -4.02 to 1.26 |
| 5 | -2.06 | 1.04 | -5.01 to 0.90 |
| 6 | -1.44 | 0.98 | -4.23 to 1.35 |
| 7 | -1.4 | 1.10 | -4.54 to 1.74 |
| 8 | -0.92 | 1.15 | -4.19 to 2.35 |
| 9 | -0.36 | 1.16 | -3.65 to 2.93 |
| 10 | -0.27 | 1.30 | -3.97 to 3.43 |
| 11 | 0.02 | 1.52 | -4.32 to 4.35 |
| 12 | 1.83 | 1.73 | -3.10 to 6.77 |
| 13 | 3.68 | 2.12 | -2.35 to 9.70 |

### 3.3 Causal Effect Estimation With a Matched Sample

Treatment effects reestimated using DID on matched sample (375 treated, 375 controls). Dynamic treatment effects showed significant eGFR decline during the early post-treatment period—at event times 0, 1, and 3—with estimates of -3.90 (95% CB: -6.20 to -1.60), -2.37 (95% CB: -4.54 to -0.20), and -2.56 (95% CB: -5.11 to -0.02), respectively. No statistically significant changes at later time points.

**Table 2 — Time-varying treatment effects estimated following propensity score matching**

| Event time (months) | Estimate (mL/min/1.73 m²) | Std. error | 95% CI |
|---|---|---|---|
| -12 | 0.50 | 0.72 | -1.55 to 2.56 |
| -11 | 0.54 | 0.58 | -1.11 to 2.19 |
| -10 | 0.14 | 0.38 | -0.93 to 1.21 |
| -9 | -0.38 | 0.53 | -1.87 to 1.12 |
| -8 | -0.25 | 0.35 | -1.23 to 0.74 |
| -7 | 0.27 | 0.45 | -1.01 to 1.56 |
| -6 | -0.37 | 0.51 | -1.82 to 1.09 |
| -5 | 0.10 | 0.43 | -1.13 to 1.33 |
| -4 | -0.67 | 0.43 | -1.91 to 0.57 |
| -3 | -0.07 | 0.37 | -1.11 to 0.97 |
| -2 | -1.16 | 0.47 | -2.50 to 0.18 |
| -1 | -0.07 | 0.39 | -1.19 to 1.06 |
| **0** | **-3.90** | **0.81** | **-6.20 to -1.60** |
| **1** | **-2.37** | **0.76** | **-4.54 to -0.20** |
| 2 | -2.29 | 0.93 | -4.94 to 0.36 |
| **3** | **-2.56** | **0.89** | **-5.11 to -0.02** |
| 4 | -1.46 | 0.99 | -4.27 to 1.36 |
| 5 | -2.22 | 1.13 | -5.43 to 0.99 |
| 6 | -1.63 | 1.1 | -4.75 to 1.49 |
| 7 | -1.64 | 1.19 | -5.04 to 1.75 |
| 8 | -1.38 | 1.23 | -4.88 to 2.13 |
| 9 | -0.84 | 1.33 | -4.62 to 2.95 |
| 10 | -0.81 | 1.62 | -5.43 to 3.81 |
| 11 | -0.51 | 1.63 | -5.15 to 4.13 |
| 12 | 1.26 | 1.92 | -4.21 to 6.73 |
| 13 | 3.09 | 2.28 | -3.39 to 9.58 |

### 3.4 Subgroup Analyses

Separate PSM was not performed within each subgroup to preserve statistical power. Causal identification relies on the parallel pre-treatment trends assumption rather than exact baseline covariate balance.

### 3.5 Presence of Proteinuria

- **Low-grade proteinuria (n = 851):** ATT was -0.13 mL/min/1.73 m² (95% CB: -2.07 to 1.81), no significant overall change. Figure 1 shows a statistically significant eGFR decline only at event time 0 (estimate: -2.33; 95% CB: -4.63 to -0.04). No significant effects at subsequent time points.
- **High-grade proteinuria (n = 353):** ATT was -5.97 mL/min/1.73 m² (95% CB: -10.99 to -0.96), statistically significant eGFR decline. Figure 2 shows significant declines beginning at event time 0 and persisting through event time 7, with notable declines at time points 0 (estimate: -7.56; 95% CB: -12.04 to -3.09), 1 (estimate: -6.50; 95% CB: -11.18 to -1.81), and times 3-7 (all statistically significant). Patients with high-grade proteinuria experience a more sustained and pronounced eGFR decline during the early treatment phase.

### 3.6 Presence of Advanced Chronic Kidney Disease

Advanced CKD subgroup (n = 873). ATT was -2.34 mL/min/1.73 m² (95% CB: -4.27 to -0.41), statistically significant decline. Dynamic effect estimates revealed significant eGFR declines at event times 0 (estimate: -3.28; 95% CB: -5.71 to -0.86) and 1 (estimate: -2.58; 95% CB: -4.81 to -0.34) (Figure S3). Although treatment effects remained negative at subsequent time points, most were not statistically significant.

---

## 4. Discussion

This study shows that eGFR declines following RAAS inhibitor initiation are transient, with no sustained renal impairment over the first year of therapy. Significant reductions in eGFR occurred only within the first 3 months, indicating the acute hemodynamic impact attenuates within the first year. The findings are consistent with previous meta-analyses and RCTs reporting stabilization of eGFR after an initial 1-3 months decline.

The initial eGFR decline reflects a hemodynamic response—reductions in systemic and intraglomerular pressure rather than structural renal injury. This functional decrease is generally reversible and may provide long-term renal protection by mitigating glomerular hypertension. A significant and rapid eGFR decline exceeding 30% may indicate excessive renal perfusion reduction and heightened risk of acute kidney injury. A large observational study reported that patients with ≥ 30% increases in serum creatinine after RAAS inhibitor initiation had significantly higher risks of ESRD and mortality. In a UK cohort, only 1.7% experienced such elevation within 2 months of starting ACEi/ARB therapy. In this treated cohort, 73 patients (19.5%) experienced a ≥ 30% decline in eGFR within the first 3 months. However, these early reductions largely represent an expected transient hemodynamic response prompting routine clinical reassessment, rather than true structural AKI, which was minimized by baseline exclusion criteria. Consistent with KDIGO guidelines recommending continuation of RAAS inhibitors unless the eGFR decline exceeds 30%, the present findings support this recommendation, showing average reductions (~6.5%) remain well within safe thresholds.

Methodological findings: Estimates from the TWFE model reflect limitations in capturing dynamic treatment effects. The staggered DID model enabled quantification of time-varying treatment effects. The parallel trend assumption was supported by CBs for all estimated coefficients before relative time point -1 including zero.

**High-grade proteinuria subgroup:** RAAS inhibitor therapy was associated with a significant and sustained early decline in eGFR, indicating a pronounced hemodynamic response. ACE inhibitors and ARBs preferentially dilate the efferent arteriole and, to a lesser extent, the afferent arteriole, thereby reducing intraglomerular pressure, hyperfiltration, and proteinuria. Patients with elevated baseline intraglomerular pressure and RAAS activity are more likely to experience a pronounced initial "functional" reduction.

**Advanced CKD subgroup:** A modest but significant reduction observed during the initial post-treatment period, with effect gradually diminishing. Consistent with Bhandari et al. reporting that discontinuing RAAS inhibitors in patients with advanced CKD did not significantly improve renal function, highlighting the limited reversibility of early eGFR declines.

**Clinical relevance:** Highlights the importance of continuing RAAS inhibitor therapy unless clinical instability or severe renal deterioration develops. Premature discontinuation may deprive patients of long-term renoprotective and cardioprotective benefits. Initial reductions do not result in progressive renal impairment within the first year and, by themselves, should not warrant discontinuing therapy.

**Limitations:**
1. Despite using staggered DID with PSM, residual confounding may persist. No active-comparator new-user design was used; confounding by indication is a potential limitation. Lack of detailed data on concurrent reno-protective medications (SGLT2 inhibitors, GLP-1 receptor agonists, MRAs) remains an unmeasured confounder.
2. Cohort restricted to patients with > 10 renal function tests over > 3 years—limits generalizability; inclusion of only two Korean hospitals limits generalizability to broader populations.
3. Analysis focused on the dynamic eGFR response during the first 12 months; relatively short follow-up prevents definitive claims regarding multi-year long-term effects.

**Conclusion:** This study strengthens the evidence that the initial decline in eGFR with RAAS inhibitor therapy represents a transient hemodynamic response rather than permanent renal injury. The staggered DID design enabled time-sensitive causal estimation, showing continued RAAS inhibition remains safe in patients with CKD when the eGFR decline is within clinically acceptable thresholds. Findings support guideline recommendations to avoid premature discontinuation of therapy and demonstrate that quasi-experimental analyses of real-world data can reproduce conclusions of RCTs and meta-analyses.

---

## Author Contributions

T.R.O. wrote the manuscript. T.R.O. designed the research. T.R.O. and J.Y.P. analyzed the data. T.R.O., J.Y.P., H.S.C., H.R.R., and G.K. performed the research.

## Acknowledgments

Declaration of generative AI in scientific writing: During preparation, the authors used Gemini (Google) to improve language and readability. The authors reviewed and edited the output and take full responsibility.

## Funding

Supported by the Biomedical Research Institute of Chonnam National University Hospital in Gwangju, Korea (Grants BCRI23036 and BCRI-25088).

## Conflicts of Interest

The authors declare no conflicts of interest.

## Data Availability Statement

The corresponding author and Tae Ryom Oh had full access to all the data.

## Supporting Information

- Table S1: Baseline characteristics of the study cohort
- Figure S1: Density plot of actual body surface area distribution
- Figure S2: Covariate balance after propensity score matching
- Figure S3: Time-varying treatment effects in patients with advanced chronic kidney disease

---

## Key References (selected)

- [12] Ku E, Tighiouart H, McCulloch CE, et al. "Association Between Acute Declines in eGFR During Renin-Angiotensin System Inhibition and Risk of Adverse Outcomes," J Am Soc Nephrol 35, no. 10 (2024): 1402-1411.
- [13] Jackevicius CA, Wong J, Aroustamian I, Gee M, Mody FV. "Rates and Predictors of ACE Inhibitor Discontinuation Subsequent to Elevated Serum Creatinine," BMJ Open 4, no. 6 (2014): e005181.
- [16] KDIGO 2024 Clinical Practice Guideline for the Evaluation and Management of CKD, Kidney International 105, no. 4S (2024): S117-S314.
- [28] Schmidt M, Mansfield KE, Bhaskaran K, et al. "Serum Creatinine Elevation After Renin Angiotensin System Blockade and Long Term Cardiorenal Risks: Cohort Study," BMJ 356 (2017): j791.
- [31] Clase CM, Barzilay J, Gao P, et al. "Acute Change in Glomerular Filtration Rate With Inhibition of the Renin-Angiotensin System Does Not Predict Subsequent Renal and Cardiovascular Outcomes," Kidney International 91, no. 3 (2017): 683-690.
- [32] Bhandari S, Mehta S, Khwaja A, et al. "Renin-Angiotensin System Inhibition in Advanced Chronic Kidney Disease," N Engl J Med 387, no. 22 (2022): 2021-2032.

---

*Source: Clinical and Translational Science, 2026; 19:e70533. https://doi.org/10.1111/cts.70533. Open access (CC BY-NC). Full text retrieved via Europe PMC.*
