---
title: "Clinical Implications of Slope of GFR in Clinical Trials of CKD Progression"
authors: "Greene T; Collier W; Haaland B; Zhang C; Badve SV; Caravaca-Fontán F; Del Vecchio L; Floege J; Hannedouche T; Imai E; Jafar TH; Lewis JB; Li PKT; Locatelli F; Maes BD; Neuen BL; Perrone RD; Schena FP; Toto R; Wanner C; Woodward M; van Zuilen A; Heerspink HJL; Inker LA (for the CKD-EPI Clinical Trials Consortium)"
year: 2025
journal: "Clinical Journal of the American Society of Nephrology (CJASN)"
doi: "10.2215/CJN.0000000662"
pmid: "40237639"
source: "Europe PMC OA (via paper-search download_with_fallback); CJASN 20:632–641, May 2025"
content_verified: true
---

# Clinical Implications of Slope of GFR in Clinical Trials of CKD Progression

**Citation:** CJASN 20: 632–641, 2025. doi: https://doi.org/10.2215/CJN.0000000662
Received: August 29, 2024; Accepted: March 12, 2025; Published Online Ahead of Print: April 15, 2025.
Correspondence: Dr. Lesley A. Inker (Lesley.Inker@tuftsmedicine.org).
For the CKD-EPI Clinical Trials Consortium.

## Key Points

- Acute effects impact the clinical endpoint independently of treatment effects on the chronic slope.
- Our findings support the 3-year total slope as the primary slope-based outcome in randomized trials.

## Abstract

**Background.** Slope of the GFR is considered a validated surrogate endpoint for CKD trials. However, differing short-term and long-term treatment effects on GFR slope can create ambiguities concerning the appropriate period for evaluating slope, in part because current methods cannot separate the distinct contributions of the acute (before 3 months) and chronic (after 3 months) slopes for treatment effects on clinical endpoints (CEs).

**Methods.** We estimated treatment effects on the acute and chronic GFR slopes and on the established CE of kidney failure or serum creatinine doubling for 66 randomized treatment comparisons from previous CKD clinical trials. We used a novel Bayesian meta-regression framework to relate treatment effects on the established CE to both the acute and chronic slopes in a single multivariable model to determine the independent contributions of the acute and chronic slopes.

**Results.** Treatment effects on both the acute and chronic slopes independently predicted the treatment effect on the established CE with a high median R² (95% credible interval) of 0.95 (0.79 to 1.00). For a fixed treatment effect on the chronic slope, each 1 ml/min per 1.73 m² greater acute GFR decline for the treatment versus control increased the hazard ratio for the established CE by 11.4% (7.9%–15.0%), against the treatment. The optimal weights for the acute and chronic slopes were consistent with the 3-year total slope defined as the average slope extending from baseline to 3 years.

**Conclusions.** Treatment effects on both the acute and chronic GFR slopes are independent determinants of the effects on the established CE, with variation in acute effects accounting for much of the observed variation in treatment effects on the CE across previous trials. Our results establish that acute effects affect the CE independently of treatment effects on the chronic slope and support the 3-year total slope as the primary slope-based outcome in randomized trials.

## Introduction

Pivotal randomized controlled trials (RCTs) for CKD traditionally use the established clinical endpoint (CE) of kidney failure with replacement therapy (KFRT), GFR <15 ml/min per 1.73 m², or doubling of serum creatinine or a similar composite of clinical events as the primary outcome. Because these are late events in CKD, RCTs in CKD often require lengthy follow-up or restriction to patients with severe disease. GFR decline is on the causal pathway to kidney failure for all kidney diseases, providing strong biologic plausibility for GFR slope as a surrogate endpoint to reduce sample size or follow-up time, and robust epidemiologic association has been demonstrated between GFR declines and subsequent kidney failure.

A challenge for application of GFR slope in CKD RCTs is the common occurrence of acute effects, usually within 3 months after treatment initiation, which differ from longer term treatment effects on the rate of GFR change after 3 months, referred to as the chronic slope. The authors have previously demonstrated that treatment effects on the established CE are predicted with higher accuracy from treatment effects on the average GFR slope over 3 years (which incorporates both the chronic slope and the acute slope, defined as the mean GFR change from baseline to 3 months, interpreted as an average slope over 3 months), than from treatment effects specifically on the chronic slope, which ignore the acute GFR change. This suggests that acute GFR changes play a role in determining effects of treatments on the established CE. However, because previous work has been limited to univariate models restricted to one slope-based endpoint at a time, it has not been possible to determine the independent contributions of the acute and chronic slopes for treatment effects on CEs.

The primary goal of this article is to relate treatment effects on the established CE to both the acute and chronic slopes in a single multivariable model to determine the independent contributions of the acute and chronic slopes, and to determine whether the average GFR slope over 3 years is the optimal slope-based endpoint from among all possible ways of weighting the acute and chronic slopes. A second goal is to apply this model to alternative time-to-event outcomes defined by progressively larger GFR declines.

## Methods

### Dataset

RCTs of CKD progression were identified using a systematic search. For RCTs that evaluated more than one intervention, a separate comparison was included for each active treatment versus the control. RCTs with <100 participants were pooled if the disease and intervention were the same. This yielded **66 randomized treatment comparisons** (called "studies") across a wide range of treatments, CKD subtypes, and disease severity. The 66 studies evaluated 17 treatment classes across four main disease categories: 24 studies consisted predominantly of diabetic patients, 10 of glomerular diseases, 28 of other kidney diseases, and 7 of cardiovascular disease patient populations at risk for kidney disease.

### Time-to-Event Endpoints

The established CE is a composite of KFRT, sustained GFR <15 ml/min per 1.73 m², or doubling of serum creatinine. A sustained GFR <15 was determined if the baseline GFR was >25 ml/min per 1.73 m² and the participant had a GFR <15 ml/min per 1.73 m² on two consecutive study visits or at the last visit. The authors also evaluated the true CE of KFRT or sustained GFR <15 ml/min per 1.73 m². Finally, they evaluated composite endpoints defined by the time to either sustained 30% and 40% GFR decline along with KFRT or sustained GFR <15 ml/min per 1.73 m². GFR was estimated using the 2009 CKD Epidemiology Collaboration (CKD-EPI) equation.

### Statistical Analyses

**Acute, Chronic, and Total GFR Slope.** Within each study, GFR slope was analyzed using a mixed effects shared parameter model with a linear slope starting 3 months after randomization while accounting for informative censoring by KFRT and death. The acute effect and the treatment effect on the chronic slope are defined by differences between randomized groups in the mean intercept at 3 months (in ml/min per 1.73 m² per 3 months) and in the mean slope after 3 months (in ml/min per 1.73 m² per year), respectively. The model assumes mean GFR declines linearly after 3 months but allows any pattern of GFR change within the first 3 months.

**Trial-Level Model.** In the first stage, treatment effects on the acute and chronic GFR slopes were estimated in each study, and treatment effects on the CE (as log hazard ratios, HRs) were estimated using Cox proportional hazards regression. Standard errors and robust sandwich estimates of the correlations between sampling errors were obtained. In the second stage, a multivariable mixed-effect Bayesian model was fit to the results, with the 66 studies as units of analysis. The key meta-regression jointly relates the treatment effects on the established CE to the treatment effects on the chronic and acute GFR slopes:

> (Log HR for CE) = (b_acute × [Acute Effect]) + (b_chronic × [Treatment effect on chronic slope]) + (b0 + [residual])

Here, b0 is the intercept, and b_acute and b_chronic are the meta-regression slope coefficients. The weighted average is supported as a valid surrogate if (1) one or both coefficients deviate substantially from 0 with Bayesian credible intervals (BCIs) that exclude 0; (2) the intercept b0 is close to 0; and (3) the trial-level R² is high (e.g., >0.72), indicating accurate prediction.

**Sensitivity Analyses.** The basic model was refit in (1) 59 of the 66 studies which included a GFR measurement between month 3 and month 6, and (2) 52 studies remaining after excluding those which evaluated immunosuppressive or dietary interventions or those conducted in heart failure patients.

**Prediction Intervals and Positive Predictive Value.** 95% Bayesian prediction intervals were computed and probabilities of clinical benefit (defined as either HR <1 or HR <0.8) were estimated, first assuming the "true" treatment effects are known without error, then assuming effects estimated from an intermediate-size 3-year trial with 600 patients per group and GFR measurements every 6 months. The posterior probabilities of clinical benefit are referred to as trial-level positive predictive value (PPV_trial).

**Model Extensions.** Linear splines were added to separately evaluate implications of positive and negative acute effects. Interactions with each study's mean baseline GFR and mean baseline log urine albumin to creatinine ratio (ACR) were added. Analyses used SAS 9.4 and R 4.3.1.

## Results

### Treatment Effects on Both the Acute and Chronic Slopes Independently Influence the Treatment Effect on the Established CE

The meta-regression coefficients for both the acute effect and the chronic slope differ substantially from 0: **−0.11 (−0.14 to −0.08) per 3 months for the acute effect** and **−0.34 (−0.43 to −0.27) per year for the chronic slope**, indicating both independently influence the treatment effect on the established CE. When expressed in common time units, the median ratio of the weights for the acute versus the chronic slope is **0.078 (0.055 to 0.105)**, similar to the ratio of weights in the 3-year total slope ([3 months]/[33 months] = 0.09). The intercept **−0.03 (−0.10 to 0.03)** indicates the treatment effect on the established CE is likely small in the absence of a treatment effect on slopes. The **R² for the joint model is 0.95 (0.79–1.00)**.

For a fixed treatment effect on chronic slope, each 1 ml/min per 1.73 m² per 3-month greater acute GFR decline for treatment versus control predicted a greater HR for the established CE of **11.4%**. For a fixed acute effect, each 0.75 ml/min per 1.73 m² per year greater treatment effect on chronic slope predicted a **22.8% lower HR**. In the extended model allowing different coefficients, a positive acute effect of 1 ml/min per 1.73 m² led to a similar shift in favor of the treatment (8.9%) as a negative acute effect of the same size against the treatment (13.1%).

Results were similar when restricted to the 59 studies with GFR between months 3 and 6, or to the 52 studies remaining after excluding diet, immunosuppressive treatments, and heart failure trials.

#### Table 1. Relationship of treatment effects on the established CE versus treatment effects on acute and chronic GFR slopes in 66 studies (posterior medians; 2.5th–97.5th percentile)

| Variable | Median | 2.5th–97.5th Percentile |
|---|---|---|
| Intercept | −0.03 | −0.10 to 0.03 |
| Chronic slope coefficient (per ml/min per 1.73² per year) | −0.34 | −0.43 to −0.27 |
| Acute effect coefficient (per ml/min per 1.73² per 3 mo) | −0.11 | −0.14 to −0.08 |
| Ratio of acute vs chronic slope coefficients (common time units) | 0.078 | 0.055 to 0.105 |
| Trial-level R² | 0.95 | 0.79 to 1.00 |
| Trial-level RMSE | 0.06 | 0.02 to 0.13 |
| Impact of 1 ml/min/1.73 m² per 3 mo greater negative acute effect (% Δ in HR) | 11.4% | 7.9% to 15.0% |
| Impact of 0.75 ml/min/1.73 m² per year greater treatment effect on chronic slope (% Δ in HR) | −22.8% | −27.7% to −18.1% |

### How the Treatment Effects on the Acute and Chronic Slopes Combined to Determine the Treatment Effect on the Established CE in Previous Studies

Figure 1 shows the distinct contributions of treatment effects on the acute and chronic slopes for the predicted HR of the established CE for each of the 66 studies. Variation in treatment effects on both slopes contributed greatly to differences in HRs for the CE across trials. Among studies with small treatment effects on the chronic slope (−0.5 to +0.5 ml/min per 1.73 m² per year), the predicted treatment effect ranged from HRs >1.2 (harmful; e.g., SPRINT, with large negative acute effects) to HR close to 0.5 (ACCOMPLISH, with a large positive acute effect). Negative acute effects were observed in the SGLT2 inhibitor studies, but their consequences were exceeded by large beneficial effects on the chronic slope, leading to predicted HRs substantially below 1.

### Implications for Study Design

95% prediction intervals (Figure 2) and PPVs show that greater beneficial effects on the chronic slope are required to infer treatment benefit on the CE for interventions with negative acute effects than for interventions with positive acute effects.

### Influence of the Acute Effect Is Reduced for Time-to-Event Endpoints Based on Larger GFR Decline

The effect of the acute slope on the CE progressively decreased for endpoints based on larger GFR decline. The median effect of a 1 ml/min per 1.73 m² per 3-month greater negative acute effect decreased from 15.3% (30% GFR decline endpoint) to 13.3%, 11.4%, and 5.7% respectively for the remaining endpoints. The impact of the acute effect remained nonzero even for the true CE (95% BCIs all excluding 0). The intercept BCI included 0 for the first three endpoints but was <0 for the true CE (−0.09 [−0.18 to −0.02]), indicating a modest average benefit on the true CE even in the absence of an effect on slopes.

#### Table 2. Comparison of results across alternative clinical endpoints defined by progressively larger GFR declines (posterior medians; 95% BCI)

| Variable | 30% GFR decline + <15 + dialysis | 40% GFR decline + <15 + dialysis | Confirmed SCr Doubling + <15 + dialysis (Established CE) | GFR <15 + dialysis (True CE) |
|---|---|---|---|---|
| Intercept | −0.03 (−0.08 to 0.01) | −0.04 (−0.09 to 0.01) | −0.03 (−0.10 to 0.03) | −0.09 (−0.18 to −0.02) |
| Chronic slope coeff (per ml/min/1.73² per yr) | −0.29 (−0.35 to −0.23) | −0.34 (−0.41 to −0.28) | −0.34 (−0.43 to −0.27) | −0.20 (−0.30 to −0.10) |
| Acute effect coeff (per ml/min/1.73² per 3 mo) | −0.14 (−0.16 to −0.12) | −0.13 (−0.15 to −0.10) | −0.11 (−0.14 to −0.08) | −0.06 (−0.10 to −0.01) |
| Trial-level R² | 0.93 (0.84 to 0.98) | 0.94 (0.85 to 0.99) | 0.95 (0.79 to 1.00) | 0.91 (0.50 to 0.99) |
| Trial-level RMSE | 0.08 (0.05 to 0.11) | 0.07 (0.03 to 0.11) | 0.06 (0.02 to 0.13) | 0.05 (0.02 to 0.11) |
| Impact of 1 ml/min/1.73 m² per 3 mo greater negative acute effect (% Δ HR) | 15.3% (12.9–17.9%) | 13.3% (10.7–16.1%) | 11.4% (7.9–15.0%) | 5.7% (1.4–10.2%) |
| Impact of 0.75 ml/min/1.73 m² per year greater treatment effect on chronic slope (% Δ HR) | −19.5% (−23.0 to −15.9%) | −22.5% (−26.5 to −18.8%) | −22.8% (−27.7 to −18.1%) | −14.2% (−20.0 to −7.5%) |

### Optimal Meta-Regression Coefficient for the Chronic Slope Depends on Baseline ACR

For a given effect on the chronic slope, the implications of the acute effect for the established CE were unrelated to mean baseline GFR and baseline ACR. However, ACR level affected the meta-regression coefficient of the chronic slope. The 95% BCI for the baseline ACR by chronic slope interaction excludes 0 (0.024 to 0.137), indicating the same treatment effect on the chronic slope translates to a larger effect on the established CE at lower baseline ACR. For example, a 0.75 ml/min per 1.73 m² per year greater treatment effect on the chronic slope translates to a 15.8% (5.1% to 24.2%) reduced HR when baseline ACR = 1000 mg/g compared with a 31.8% (23.1% to 38.1%) reduced HR when baseline ACR = 30 mg/g.

#### Table 3. Interaction models with baseline GFR and baseline log ACR as continuous variables (posterior medians; 95% BCI)

**Panel A: interactions with baseline GFR**

| Variable | Median (95% BCI) | Impact of 0.75 ml/min/1.73 m² greater treatment effect on chronic slope (% Δ HR for established CE) |
|---|---|---|
| Interaction of acute effect coeff with baseline GFR | 0.000 (−0.005 to 0.005) | NA |
| Interaction of chronic slope coeff with baseline GFR | −0.016 (−0.081 to 0.040) | NA |
| Chronic slope coeff at baseline GFR = 30 | −0.31 (−0.49 to −0.10) | −20.7% (−30.8% to −7.2%) |
| Chronic slope coeff at baseline GFR = 60 | −0.35 (−0.46 to −0.26) | −23.1% (−29.2% to −17.7%) |
| Chronic slope coeff at baseline GFR = 90 | −0.40 (−0.62 to −0.20) | −25.9% (−37.2% to −13.9%) |

**Panel B: interactions with baseline ACR**

| Variable | Median (95% BCI) | Impact of 0.75 ml/min/1.73 m² greater treatment effect on chronic slope (% Δ HR for established CE) |
|---|---|---|
| Interaction of acute effect coeff with baseline Log(ACR) | −0.002 (−0.007 to 0.004) | NA |
| Interaction of chronic slope coeff with baseline Log(ACR) | 0.079 (0.024 to 0.137) | NA |
| Chronic slope coeff at baseline ACR = 30 mg/g | −0.51 (−0.64 to −0.35) | −31.8% (−38.1% to −23.1%) |
| Chronic slope coeff at baseline ACR = 150 mg/g | −0.38 (−0.48 to −0.27) | −24.8% (−30.2% to −18.3%) |
| Chronic slope coeff at baseline ACR = 1000 mg/g | −0.23 (−0.37 to −0.07) | −15.8% (−24.2% to −5.1%) |

## Discussion

This article extends previous models for validating individual surrogate endpoints to a new multivariable framework that quantifies the independent contributions of the acute and chronic slopes for determining treatment effects on CEs. The analysis demonstrates that treatment effects on both the acute and chronic slopes are strong, independent predictors of the treatment effect on the established CE (doubling serum creatinine, GFR <15 ml/min per 1.73 m², or dialysis). Most importantly, among studies conducted to date, the **3-year total slope provides near optimal prediction** among all possible endpoints constructed as weighted averages of the acute and chronic slopes, supporting its use as the primary slope-based outcome in randomized trials.

The multivariable analyses confirm that the acute effect has substantial clinical implications distinct from the chronic slope: for a fixed treatment effect on the chronic slope, each 1 ml/min per 1.73 m² per 3-month greater acute GFR decline increases the HR for the CE by 11.4% against the treatment. Thus, larger beneficial effects on the chronic slope are required to demonstrate benefit on the CE when the acute effect is negative than when it is absent or positive.

The influence of the acute effect persisted when the analysis was repeated for the true CE (KFRT or sustained GFR decline to 15 ml/min per 1.73 m²). This likely reflects that, given the same treatment effect on the chronic slope, patients with a greater acute GFR decline tend to have lower average GFR and hence an increased probability of reaching the low GFR levels that trigger KFRT. Nevertheless, the contribution of the acute effect was reduced by about half for the true CE compared with the established CE, suggesting that including doubling serum creatinine events in the established CE may overstate the role of the acute effect for progression to kidney failure. Trials using the established CE may thus provide conservative assessments of clinical benefit for interventions with large negative acute effects.

There was no evidence that the level of GFR affected the relationship between treatment effects on the acute and chronic slopes with treatment effects on the CE, indicating the same weights can be applied at all CKD stages. However, the coefficient relating the chronic slope to the log HR for the CE increased at lower baseline ACR, associated with slower GFR decline.

**Limitations.** (1) Prediction intervals for a future trial assume the relationship between treatment effects on slope and CEs is similar between the future trial and previous trials. (2) Simulation studies have shown that GFR slope reduces sample size requirements compared with the established CE in many but not all situations. (3) The analyses evaluated the association over the follow-up periods of trials in the database; the importance of the acute slope might diminish if CEs were evaluated over extended time horizons. (4) The article addresses the implications of different acute effects specifically among trials with the same treatment effects on the chronic slope.

**Conclusion.** The authors extended previous models for evaluating individual surrogate endpoints to a multivariable framework that resolves the independent contributions of the acute and chronic GFR slopes. This approach supports the validity of the 3-year total slope as a primary endpoint for slope-based CKD RCTs, with both the acute and chronic slopes making substantial independent contributions to prediction of the treatment effect on the established CE.

## Data Sharing / Code

Statistical code for the primary analysis: https://github.com/UofUEpiBio/ckdepict
Datasets requested through Vivli, NIDDK, NHLBI BioLINCC, Clinical Study Data Request, and sponsors' websites (see Supplemental Appendix 1). Trials referenced include CANVAS, CANVAS-R, CREDENCE, EMPA-REG Outcome, EXAMINE, Harmony Outcome, FIDELIO-DKD, AASK, FSGS/FONT, HALT-PKD A and B, MDRD, TOPCAT, SPRINT, PARADIGM-HF, ACCOMPLISH, LEADER.

## Funding

Supported by the National Kidney Foundation through sponsorship agreements with Alexion Pharmaceuticals, AstraZeneca United States, Bayer, Boehringer Ingelheim, CSL Behring, Novartis Pharmaceuticals Corporation, Novo Nordisk A/S, ProKidney, Roche/Genentech, and Travere. Additional support from the Utah Study Design and Biostatistics Center (NIH NCATS UL1TR002538).

## Selected References

1. Coresh J, Turin TC, Matsushita K, et al. Decline in estimated glomerular filtration rate and subsequent risk of end-stage renal disease and mortality. JAMA. 2014;311(24):2518–2531. doi:10.1001/jama.2014.6634
2. Grams ME, Sang Y, Ballew SH, et al. Evaluating glomerular filtration rate slope as a surrogate end point for ESKD in clinical trials: an individual participant meta-analysis of observational data. J Am Soc Nephrol. 2019;30(9):1746–1755. doi:10.1681/ASN.2019010008
4. Levey AS, Inker LA, Matsushita K, et al. GFR decline as an end point for clinical trials in CKD: a scientific workshop sponsored by the NKF and the US FDA. Am J Kidney Dis. 2014;64(6):821–835. doi:10.1053/j.ajkd.2014.07.030
6. Inker LA, Heerspink HJL, Tighiouart H, et al. GFR slope as a surrogate end point for kidney disease progression in clinical trials: a meta-analysis of treatment effects of randomized controlled trials. J Am Soc Nephrol. 2019;30(9):1735–1745. doi:10.1681/ASN.2019010007
8. Inker LA, Collier W, Greene T, et al. A meta-analysis of GFR slope as a surrogate endpoint for kidney failure. Nat Med. 2023;29(7):1867–1876. doi:10.1038/s41591-023-02418-0
16. Heerspink HJ, Inker LA, Tighiouart H, et al. Change in albuminuria and GFR slope as joint surrogate end points for kidney failure: implications for phase 2 clinical trials in CKD. J Am Soc Nephrol. 2023;34(6):955–968. doi:10.1681/ASN.0000000000000117
17. Ku E, Bakris G, Johansen KL, et al. Acute declines in renal function during intensive BP lowering: implications for future ESRD risk. J Am Soc Nephrol. 2017;28(9):2794–2801. doi:10.1681/ASN.2017010040
18. Heerspink HJ, Eddington D, Chaudhari J, et al. A meta-analysis of randomized controlled clinical trials for implications of acute treatment effects on glomerular filtration rate for long-term kidney protection. Kidney Int. 2024;106(4):688–698. doi:10.1016/j.kint.2024.05.024

---

*Full text retrieved and human-verified (title, authors, journal, DOI, PMID all consistent with source metadata). Source: Europe PMC OA PDF, CJASN 20:632–641, May 2025.*
