---
title: "Risk and treatment effect heterogeneity: re-analysis of individual participant data from 32 large clinical trials"
authors: "David M. Kent; Jason Nelson; Issa J. Dahabreh; Peter M. Rothwell; Douglas G. Altman; Rodney A. Hayward"
year: 2016
journal: "International Journal of Epidemiology"
volume: "45"
issue: "6"
pages: "2075-2088"
doi: "10.1093/ije/dyw118"
pmid: "27375287"
pmcid: "PMC5841614"
source: "Europe PMC (PMC5841614, publisher PDF via europepmc.org render) — full text verified"
content_verified: true
---

# Risk and treatment effect heterogeneity: re-analysis of individual participant data from 32 large clinical trials

**Authors:** David M Kent,¹* Jason Nelson,¹ Issa J Dahabreh,¹,²,³,⁴ Peter M Rothwell,⁵ Douglas G Altman,⁶ Rodney A Hayward⁷

¹ Predictive Analytics and Comparative Effectiveness (PACE) Center, Tufts Medical Center/Tufts University School of Medicine, Boston, MA, USA
² Center for Evidence-Based Medicine, ³ Department of Health Services, Policy & Practice, ⁴ Department of Epidemiology, Brown University, Providence, RI, USA
⁵ Stroke Prevention Research Unit, Nuffield Department of Clinical Neuroscience, University of Oxford, Oxford, UK
⁶ Centre for Statistics in Medicine, Nuffield Department of Orthopaedics, Rheumatology & Musculoskeletal Sciences, University of Oxford, Oxford, UK
⁷ Department of Internal Medicine and Department of Health Management and Policy, University of Michigan, Ann Arbor, MI, USA

*Corresponding author:* dkent1@tuftsmedicalcenter.org
Accepted 18 April 2016; Advance Access Publication 3 July 2016.

*Article type: Original article — Methodological insights.*

---

## Abstract

**Background:** Risk of the outcome is a mathematical determinant of the absolute treatment benefit of an intervention, yet this can vary substantially within a trial population, complicating the interpretation of trial results.

**Methods:** We developed risk models using Cox or logistic regression on a set of large publicly available randomized controlled trials (RCTs). We evaluated risk heterogeneity using the **extreme quartile risk ratio (EQRR**, the ratio of outcome rates in the lowest risk quartile to that in the highest) and skewness using the **median-to-mean risk ratio (MMRR**, the ratio of risk in the median risk patient to the average). We also examined heterogeneity of treatment effects (HTE) across risk strata.

**Results:** We describe **39 analyses using data from 32 large trials**, with event rates across studies ranging from **3% to 63%** (median = 15%, 25th–75th percentile = 9–29%). C-statistics of risk models ranged from **0.59 to 0.89** (median = 0.70, 25th–75th percentile = 0.65–0.71). The **EQRR ranged from 1.8 to 50.7** (median = 4.3, 25th–75th percentile = 3.0–6.1). The **MMRR ranged from 0.4 to 1.0** (median = 0.86, 25th–75th percentile = 0.80–0.92). EQRRs were predictably higher and MMRRs predictably lower as the c-statistic increased or the overall outcome incidence decreased. Among **18 comparisons with a significant overall treatment effect, there was a significant interaction between treatment and baseline risk on the proportional scale in only one.** The difference in the absolute risk reduction between extreme risk quartiles ranged from **3.2 to 28.3%** (median = 5.1%; 25th–75th percentile = 0.3–10.9).

**Conclusions:** There is typically substantial variation in outcome risk in clinical trials, commonly leading to clinically significant differences in absolute treatment effects. Most patients have outcome risks lower than the trial average reflected in the summary result. Risk-stratified trial analyses are feasible and may be clinically informative, particularly when the outcome is predictable and uncommon.

**Key words:** Risk prediction, heterogeneity of treatment effect, subgroup analysis, personalized medicine, patient-centered outcomes research

---

## Key Messages

- Outcome risk is a mathematical determinant of the treatment effect yet can vary substantially across a trial population, making it unclear how treatment effects might vary in the trial population.
- Using simple risk models based on baseline patient characteristics, among a sample of trials from publicly available sources, we found that outcome rates in the highest risk quartile were as high as **50-fold** those in the lowest risk quartile; in fully a quarter of the trials, this ratio exceeded 6.
- Because outcome risk in the trials was generally skewed (log-normal or logistic-normal), with a small group of high-risk patients accounting for a large number of outcomes, the outcome risk in most patients was almost always less than that reflected by the trial summary results.
- Whereas we did not often detect treatment effect heterogeneity on the proportional scale across patients at different baseline risk in this set of trials, substantial differences in absolute treatment effects were common; differences in absolute treatment effects between the extreme quartiles of risk **exceeded 10% in a quarter of trials that showed benefit**.
- Displaying results across subgroups defined by risk is feasible and can lead to clinically important findings.

---

## Introduction

A fundamental incongruity in evidence-based medicine (EBM) is that evidence is derived from groups of people yet medical decisions are made for individuals. Popular approaches to EBM have encouraged the direct application of average effects estimated in clinical trials to guide decision making for individuals, as though all patients meeting trial inclusion criteria are likely to experience similar effects from treatments.

The most commonly used method of examining whether treatment effects vary is to serially divide patients into subgroups based on pre-treatment characteristics. The main problem: there are too many potentially influential characteristics, leading to myriad "one-variable-at-a-time" subgroup analyses that are typically both underpowered and vulnerable to false-positive results due to multiple comparisons. Subgroup analyses are usually "exploratory" and rarely actionable. EBM is thus methodologically canalized to "one-size-fits-all" recommendations.

The authors previously proposed a framework for assessing HTE (Kent et al., *Trials* 2010;11:85) that prioritizes analysis and reporting of **multi-variable risk-based HTE**, and suggests that other subgroup analyses be explicitly labelled either as primary (well-motivated by prior evidence, intended to be clinically actionable) or secondary/exploratory (to inform future research). The framework is novel in suggesting that presenting summary results without examining how treatment effects change across subgroups with heterogeneous outcome risk is under-utilizing trial data and tantamount to incompletely reporting trial results. This paper examines the distribution of outcome risk across a broad range of trials and how therapy effects relate to that risk.

---

## Methods

### Data sources and eligibility
Searched publicly available individual participant datasets of RCTs from:
- National Heart, Lung, and Blood Institute (NHLBI) — BioLINCC
- National Institute of Diabetes and Digestive and Kidney Diseases (NIDDK)
- The journal *Trials*
- GlaxoSmithKline (clinicalstudydatarequest.com)

Eligible studies: enrolled at least **1000 participants** (some subcohorts had fewer than 1000), randomized to at least two treatment groups, with a **binary or time-to-event clinical (non-surrogate) outcome**.

### Predicting outcome risk using baseline covariates
- Risk modelling for each trial was informed by previously published predictive models "matched" to each trial on the basis of index condition and primary outcome (Tufts PACE clinical prediction model database).
- Because trial datasets were often incompatible with externally developed models, **"internal models" were developed on the trial data** using predictors as close as possible to those in published models. A separate simulation study (Burke et al., *Circ Cardiovasc Qual Outcomes* 2014;7:163–69) verified internal models yield results similar to external models.
- **Both trial arms were used in model development, without the treatment assignment indicator**, to avoid differential model fit between arms (which could induce a spurious risk-by-treatment interaction).
- Non-significant predictors were ranked and removed until **no more than 20 variables** entered the model (needed in only 3 of the 32 trials). No other formal variable selection or re-specification.
- For trials with non-significant primary but significant secondary outcome, an additional model was fit for the secondary outcome.
- Multivariate normal multiple imputation used when complete-case analysis would exclude >5% of participants. Predictors missing in >20% of participants were not used.
- Analysis model: Cox proportional hazards (time-to-event) or logistic regression (binary), selected on the basis of the trial's primary analysis.
- Model performance: discrimination via **c-statistic**; calibration via calibration plots; overfitting via bootstrap validation and events-per-variable.

### Risk heterogeneity metrics
- **Extreme quartile risk ratio (EQRR):** population stratified into equal quartiles by baseline predicted risk; ratio of predicted outcome risk in extreme quartiles (high-risk quartile probability ÷ low-risk quartile probability = EQRR_predicted). Also computed for observed rates (EQRR_observed). Greater values = greater risk heterogeneity.
- **Median-to-mean risk ratio (MMRR):** ratio of median predicted outcome probability to mean predicted probability; a clinically interpretable measure of skewness. Deviation from 1 reflects how much the summary (average) result may not reflect effects in the "typical" patient.
- Also computed **Pearson's median skewness coefficient (PMSC)** = 3×(mean−median)/standard deviation.
- Relationship between outcome prevalence, c-statistic, EQRR and MMRR examined visually and via linear regression.

### Evaluating HTE over predicted outcome risk
- Treatment effects estimated within each risk quartile on relative (odds ratios via logistic; hazard ratios via Cox) and absolute (absolute risk reduction via linear probability models; Kaplan–Meier survival difference for time-to-event) scales.
- HTE tested via a product ("interaction") term between the fitted linear predictor (from the risk model) and treatment assignment.
- Relative and absolute risk reduction compared between extreme risk quartiles.
- Software: SAS 9.3, R 3.1.2, Stata 13.1.

---

## Results

### Trials included
A total of **32 trials met inclusion criteria** (mostly cardiovascular: atrial fibrillation, coronary heart disease, acute MI, heart failure, hypertension, acute stroke; also prediabetes, acute kidney failure, chronic hepatitis C, prostatic hyperplasia). Patients in analysed cohorts ranged from **715 to 33,357**, totalling **180,291**. Trials published between **1979 and 2008**.

Special structure:
- One trial had more than one patient cohort (DCCT)
- One trial had more than one primary outcome (IST)
- Five trials had non-significant primary but significant secondary outcome (ACCORD, ALLHAT HTN, BEST, DIG, SOLVD)
- → **39 separate risk models** developed.

Model characteristics (Table 2):
- Median number of risk factors = 10 (average 10.9; range 4–20)
- Median events per variable = 51.3 (average 107.0; range 12.5–907.1) → models unlikely to overfit
- Median c-statistic = 0.69 (average 0.70; range 0.59–0.89)
- Bootstrap optimism-corrected c-statistics: 0.58–0.88 (median 0.68, 25th–75th percentile 0.64–0.70)
- Difference between original and optimism-corrected c-statistics: 0.001–0.02 (median 0.007) → absence of substantial overfitting

### Distribution of predicted outcome risk
- Median overall event rate = **15%** (average 20%; range 3–63%)
- Median EQRR_observed ≈ 4; **more than a quarter had EQRR_observed over 6, range extended to 50**. EQRR_predicted corresponded closely.
- Median MMRR = 0.86 (typical patient at 86% of the average outcome risk); ranged as low as 0.4; **only twice exceeded 1** (ATN, IST 6-month outcome), both trials with high outcome rates (52.6% in ATN, 62.6% in IST).
- Outcome rate and c-statistic strongly predicted the risk distribution: linear regression predicted **EQRR (R² = 0.86)** and **MMRR (R² = 0.78)** (Table 3).
- As discrimination improved and overall outcome rate was lower, EQRR increased and MMRR decreased predictably. Risk distributions were close to log-normal (Cox) or logistic-normal (logistic), so knowing outcome incidence + c-statistic essentially determines the full predicted-risk distribution.

**Table 2 — Summary of results for 39 risk distributions**

| Metric | Median | 25th–75th percentile | Mean | Range |
|---|---|---|---|---|
| Overall event rate | 0.15 | 0.09–0.29 | 0.20 | 0.03–0.63 |
| Model risk predictors | 10 | 7–16 | 10.9 | 4–20 |
| Events per variable | 51.3 | 32.3–84.7 | 107.0 | 12.5–907.1 |
| c-statistic | 0.69 | 0.65–0.71 | 0.70 | 0.59–0.89 |
| EQRR observed | 4.3 | 3.0–6.1 | 6.1 | 1.8–50.7 |
| EQRR predicted | 4.0 | 3.1–5.4 | 5.3 | 1.9–35.2 |
| MMRR | 0.86 | 0.80–0.92 | 0.84 | 0.42–1.04 |
| PMSC | 0.74 | 0.60–0.86 | 0.70 | 0.24–1.56 |

**Table 3 — Regression model results**

*log EQRR predicted (R² = 0.86):* Intercept 3.88 (SE 0.39); Overall event rate −1.94 (SE 0.24); c-statistic 8.27 (SE 0.57); all P<0.0001.
*MMRR (R² = 0.78):* Intercept 1.80 (SE 0.12); Overall event rate 0.66 (SE 0.07); c-statistic −1.57 (SE 0.17); all P<0.0001.

*(Signs per the discussion: higher c-statistic and lower event rate → higher EQRR, lower MMRR.)*

### HTE over predicted outcome risk
- Among the **18 trials with statistically non-significant overall results**, two showed statistically significant HTE over the estimated linear predictor:
  - **AMIS:** high-risk acute MI patients got more benefit from aspirin than low-risk patients (P = 0.02) on the proportional scale.
  - **IST** (death or dependency at 6 months): low-risk patients obtained more benefit than high-risk patients (P = 0.04) on the proportional scale.
- Among the **14 trials with statistically significant results, 18 unique treatment comparisons** were analysed. No apparent overall relationship between baseline risk and the hazard/odds ratio across trials. Median ratio of the HR/OR in Q4 over Q1 = **1.02** (25th–75th percentile 0.70–1.21).
- **Statistically significant interaction between treatment and the estimated linear predictor on the proportional scale in only 1 of 18 analyses** — **DPP (metformin vs placebo)**; high-risk patients experienced greater benefit than low-risk patients (P = 0.0008).
- Despite absence of "statistically significant" proportional-scale HTE, **absolute risk reduction varied substantially** and was generally higher in high-risk strata:
  - First (lowest) quartile ARR: 1.4% to 18.3% (median 4.7%; 25th–75th percentile 0.8–6.1%)
  - Fourth (highest) quartile ARR: 0.8% to 35.0% (median 9.0%; 25th–75th percentile 3.3–19.8%)
  - **Difference in ARR between extreme quartiles: 3.2% to 28.3% (median 5.1%; 25th–75th percentile 0.3–10.9)**

**Table 4 — Summary of results for 18 positive treatment comparisons (14 trials)**

| Metric | Median | IQR | Mean | Range |
|---|---|---|---|---|
| Hazard (or odds) ratio Q1 | 0.63 | 0.52–0.87 | 0.66 | 0.16–1.10 |
| Hazard (or odds) ratio Q4 | 0.69 | 0.44–0.90 | 0.64 | 0.27–0.96 |
| Extreme quartile relative hazard ratio (Q4/Q1) | 1.02 | 0.70–1.21 | 1.05 | 0.41–1.82 |
| Absolute risk reduction Q1 (%) | 4.73 | 0.83–6.06 | 4.50 | 1.43–18.27 |
| Absolute risk reduction Q4 (%) | 9.04 | 3.25–19.84 | 12.01 | 0.77–34.99 |
| Extreme quartile ARR difference (Q4−Q1) | 5.10 | 0.33–10.91 | 7.51 | 3.23–28.33 |

---

## Discussion

Clinically significant risk heterogeneity is common even in phase III "efficacy" trials often characterized as enrolling relatively homogeneous populations. Statistically significant HTE on the proportional scale was unusual in this set of trials (in which interventions generally did not have anticipated harms on the primary outcome), but variability in risk often gave rise to substantial HTE on the absolute risk scale. Absolute risk reduction (and its inverse, the number needed to treat) are generally considered the most relevant scales for clinical decision making.

Among treatment comparisons with statistically significant overall results, **25% showed differences in absolute risk differences greater than 10% between the extreme quartiles of predicted risk**. Two trials (MTOPS, DPP), encompassing 5 of the 18 treatment comparisons, were considered of sufficient clinical interest to report in separate manuscripts (Sussman et al., *BMJ* 2015;350:h454; Kozminski et al., *BJU Int* 2015;115:308–16).

**MMRR < 1 (median predicted risk lower than mean):** because trial summary results reflect arithmetic mean risk rather than median risk, the typical patient is often at lower — sometimes much lower — risk than the overall result implies. When proportional effects are similar across risk groups, summary results tend to overestimate the degree of benefit on the absolute scale — especially germane when outcome rates are predictable and relatively low.

Results were somewhat less extreme than previous published examples might suggest, for several reasons: (1) risk heterogeneity may be restricted in large phase III studies enrolling homogeneous populations; (2) simpler models were favoured to limit overfitting, yielding modest discrimination; (3) previously published examples may be "cherry-picked" for extreme results. Also, using finer grouping (quintiles/deciles) would yield more extreme ratios than quartile-based EQRRs.

**Predictability example:** using the simple linear regression results, when the outcome rate is 10% and c-statistic is 0.8, the EQRR would be approximately 13 and the MMRR approximately 0.6. When risk differs 13-fold between large population subsets, the overall trial treatment effect is not clinically interpretable. Higher c-statistics and lower outcome prevalence yield more skewed distributions and greater risk heterogeneity. A risk-stratified approach is especially important when the outcome is predictable from easily available clinical information and the overall outcome rate is low — enabling identification of very-low-risk patients unlikely to benefit; also more useful for risky or costly therapies.

Even though only DPP showed a "statistically significant" interaction, the authors urge caution in interpreting ostensible consistency of effects on the multiplicative scale: the true risk–effect relationship is underdetermined by the data, and trial results may be statistically consistent with homogeneous effects on both additive and multiplicative scales despite their mathematical incompatibility. Consistency of effects across any scale is unlikely to represent the "true" risk–effect relationship.

### Limitations
- Use of quartiles is arbitrary and tends to underestimate heterogeneity vs finer strata or smooth functions.
- Heterogeneity may be slightly overestimated (overfitting) or underestimated (underfitting); more careful model building could suggest more extreme heterogeneity.
- Non-linear relationships between risk and treatment effect were not explored (may have revealed additional HTE).
- Only a single model per trial; different models may fit equally well but yield different HTE results depending on included variables/effect modifiers.
- Convenience sample of large trials, not representing the full spectrum of conditions — particularly those where treatment can both prevent and cause the primary outcome (where more HTE would be anticipated).

### Summary
Predicted risk distributions from Cox and logistic regression are largely determined by c-statistic and outcome rates. Clinically significant risk heterogeneity is common even in large "efficacy" trials — particularly when outcome rates are low and c-statistics are high. Median risk is generally lower than average risk. Statistically significant HTE on the relative risk scale is unusual, but clinically significant heterogeneity in absolute effects appears common. A risk-stratified approach to trial analysis is feasible and may be most clinically informative when an uncommon outcome is predictable by baseline covariates.

---

## Funding
Patient-Centered Outcomes Research Institute (PCORI) Pilot Project Program Award (IP2PI000722), PCORI Methods Research Award (ME-1306-03758), and NIH (U01NS086294, UL1 TR001064).

## Conflict of interest
No authors have any disclosures to report.

---

## Trials analysed (Table 1 — 32 trials / 33 cohorts; 39 risk distributions)

ACCORD, AFFIRM, ALLHAT HTN, ALLHAT LLT, AMIS, ATN, BARI, BEST, BHAT, CAST, CPPT, DCCT (two cohorts), DIG, DPP, ENRICHD, FAVORIT, FUTURA, HALT-C, HDFP, HEMO, IST (two primary outcomes), MAGIC, MRFIT, MTOPS, OAT, PEACE, ROC (Hypertonic Saline — HS and Traumatic Brain Injury — TBI cohorts), SHEP, SOLVD, TIMI-II.

*Total patients randomized across the set: 180,291.*

---

## Selected key references cited
1. Rothwell PM. Can overall results of clinical trials be applied to all patients? *Lancet* 1995;345:1616–19.
5. Kent DM, Hayward RA. Limitations of applying summary results of clinical trials to individual patients: the need for risk stratification. *JAMA* 2007;298:1209–12.
7. Kent DM, Rothwell PM, Ioannidis JP, Altman DG, Hayward RA. Assessing and reporting heterogeneity in treatment effects in clinical trials: a proposal. *Trials* 2010;11:85.
15. Burke JF, Hayward RA, Nelson JP, Kent DM. Using internally developed risk models to assess heterogeneity in treatment effects in clinical trials. *Circ Cardiovasc Qual Outcomes* 2014;7:163–69.
18. Ioannidis JP, Lau J. Heterogeneity of the baseline risk within patient populations of clinical trials: a proposed evaluation algorithm. *Am J Epidemiol* 1998;148:1117–26.
34. Sussman JB, Kent DM, Nelson JP, Hayward RA. Improving diabetes prevention with benefit based tailored treatment: risk based reanalysis of Diabetes Prevention Program. *BMJ* 2015;350:h454.
47. Vickers AJ, Kent DM. The Lake Wobegon effect: Why most patients are at below-average risk. *Ann Intern Med* 2015;162:866–67.
49. Hayward RA, Kent DM, Vijan S, Hofer TP. Multivariable risk prediction can greatly enhance the statistical power of clinical trial subgroup analysis. *BMC Med Res Methodol* 2006;6:18.
