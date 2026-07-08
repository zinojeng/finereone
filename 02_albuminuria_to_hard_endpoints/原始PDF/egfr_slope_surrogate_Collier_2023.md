---
title: "Evaluation of Variation in the Performance of GFR Slope as a Surrogate End Point for Kidney Failure in Clinical Trials that Differ by Severity of CKD"
authors: "Collier W; Inker LA; Haaland B; Appel GB; Badve SV; Caravaca-Fontán F; Chalmers J; Floege J; Goicoechea M; Imai E; Jafar TH; Lewis JB; Li PKT; Locatelli F; Maes BD; Neuen BL; Perrone RD; Remuzzi G; Schena FP; Wanner C; Heerspink HJL; Greene T; and the Chronic Kidney Disease Epidemiology Collaboration (CKD-EPI)"
year: 2023
journal: "Clinical Journal of the American Society of Nephrology (CJASN)"
doi: "10.2215/CJN.0000000000000050"
pmid: "36754007"
volume: "18"
issue: "2"
pages: "183-192"
source: "Europe PMC (OA full text via download_with_fallback); verified against title/authors/abstract metadata"
content_verified: true
---

# Evaluation of Variation in the Performance of GFR Slope as a Surrogate End Point for Kidney Failure in Clinical Trials that Differ by Severity of CKD

**CJASN 18: 183–192, 2023. doi: https://doi.org/10.2215/CJN.0000000000000050**

Willem Collier, Lesley A. Inker, Benjamin Haaland, Gerald B. Appel, Sunil V. Badve, Fernando Caravaca-Fontán, John Chalmers, Jürgen Floege, Marian Goicoechea, Enyu Imai, Tazeen H. Jafar, Julia B. Lewis, Philip K.T. Li, Francesco Locatelli, Bart D. Maes, Brendon L. Neuen, Ronald D. Perrone, Giuseppe Remuzzi, Francesco P. Schena, Christoph Wanner, Hiddo J.L. Heerspink, Tom Greene, and the Chronic Kidney Disease Epidemiology Collaboration (CKD-EPI)

Correspondence: Dr. Lesley A. Inker, Division of Nephrology, Tufts Medical Center, 800 Washington St., Box #391, Boston, MA 02111. Email: LInker@tuftsmedicalcenter.org

---

## Abstract

**Background** The GFR slope has been evaluated as a surrogate end point for kidney failure in meta-analyses on a broad collection of randomized controlled trials (RCTs) in CKD. These analyses evaluate how accurately a treatment effect on GFR slope predicts a treatment effect on kidney failure. We sought to determine whether severity of CKD in the patient population modifies the performance of GFR slope.

**Methods** We performed Bayesian meta-regression analyses on 66 CKD RCTs to evaluate associations between effects on GFR slope (the chronic slope and the total slope over 3 years, expressed as mean differences in ml/min per 1.73 m²/yr) and those of the clinical end point (doubling of serum creatinine, GFR <15 ml/min per 1.73 m², or kidney failure, expressed as a log-hazard ratio), where models allow interaction with variables defining disease severity. We evaluated three measures (baseline GFR in 10 ml/min per 1.73 m², baseline urine albumin-to-creatinine ratio [UACR] per doubling in mg/g, and CKD progression rate defined as the control arm chronic slope, in ml/min per 1.73 m²/yr) and defined strong evidence for modification when 95% posterior credible intervals for interaction terms excluded zero.

**Results** There was no evidence for modification by disease severity when evaluating 3-year total slope (95% credible intervals for the interaction slope: baseline GFR [−0.05 to 0.03]; baseline UACR [−0.02 to 0.04]; CKD progression rate [−0.07 to 0.02]). There was strong evidence for modification in evaluations of chronic slope (95% credible intervals: baseline GFR [0.02 to 0.11]; baseline UACR [−0.11 to −0.02]; CKD progression rate [0.01 to 0.15]).

**Conclusions** These analyses indicate consistency of the performance of total slope over 3 years, which provides further evidence for its validity as a surrogate end point in RCTs representing varied CKD populations.

---

## Introduction

A critical challenge in the design of randomized controlled trials (RCTs) in CKD is that the established clinical end point, typically a composite of time-to-kidney failure with replacement therapy or doubling of serum creatinine, involves late-stage events and often takes many years to observe for patients with early-stage or slowly progressing disease. High-quality surrogate end points are thus crucial to expanding feasibility of RCTs in CKD. In some circumstances, the slope of the GFR may reveal clinically meaningful effects of therapy with shorter follow-up or smaller sample size. Meta-analyses of previously conducted CKD RCTs have demonstrated strong potential for GFR slope-based end points to be used to predict treatment effects on clinical end points.

The Chronic Kidney Disease Epidemiology Collaboration (CKD-EPI) collection of RCTs used for evaluations of GFR slope includes a spectrum of patient population CKD severities. This heterogeneity raises the question of whether there is a consistent relationship between treatment effects on GFR slope and treatment effects on the clinical end point across trials that differ by CKD severity. Previously, heterogeneity in the behavior of GFR slope as a surrogate was examined informally in a smaller set of studies by performing separate analyses in subgroups of trials defined by GFR or albuminuria thresholds. These analyses suffered from reduced statistical power due to small numbers of trials within subgroups and failed to account for the remaining heterogeneity across trials within subgroups. Analyzing severity measures as continuous in model fitting may increase statistical power and provide a more granular assessment of surrogate end point performance.

For this paper, we performed analyses using an expanded collection of 66 trials to rigorously investigate whether trial-level associations of treatment effects on the clinical and slope-based end points are modified by three measures of disease severity: baseline GFR, baseline albuminuria, and rate of CKD progression, approximated as the mean chronic slope in the control arm. We consider and contrast analyses using two different GFR slope-based end points: the total slope over a 3-year follow-up period and the chronic slope starting at 3-months follow-up. These analyses are intended to facilitate more targeted interpretation of treatment effects on slope-based end points, which will be beneficial for design and interpretation of future trials.

---

## Methods

### Data Description

A pooled database of RCTs comprising individual patient data was used. We identified trials through a systematic review of the literature. Search terms, inclusion and exclusion criteria, and bias assessment have been previously published. After applying inclusion and exclusion criteria, there were 66 randomized treatment comparisons as the main unit of analysis. For analyses using baseline albuminuria, four studies were removed due to lack of albuminuria measurements.

### End Points and Estimation of Treatment Effects

The clinical end point was defined as the first occurrence of any of the following: initiating dialysis or receiving a kidney transplant, sustained GFR below 15 ml/min per 1.73 m², or doubling of serum creatinine. Treatment effects on the clinical end point were expressed as log-hazard ratios (HRs) estimated using proportional hazards regression.

We estimated GFR using the 2009 CKD-EPI creatinine equation (eGFR, expressed in ml/min per 1.73 m²) and estimated treatment effects on GFR slope as well as standard errors using a shared parameter mixed effects model. Interventions in CKD can cause a short-term change in GFR that may differ from the long-term effect. To allow for a short-term acute treatment effect, the mixed effects model allows for a nonlinear acute GFR response up to 3 months after baseline and allows for a potentially different linear mean GFR slope thereafter. Under this model, the differences between the randomized groups in mean change from baseline to 3 months, mean slopes from 3 months onward, and mean changes from baseline to a given follow-up time of interest are defined as treatment effects on the acute, chronic, and total GFR slopes, respectively (expressed in ml/min per 1.73 m²/yr). This model allows estimation of the mean total slope over a given follow-up of interest, which we define as a time-weighted average of the mean acute and chronic slopes. Our prior analyses have demonstrated that treatment effects calculated under this model for total GFR slope over 3 years (herein total slope) and chronic GFR slope (herein chronic slope) can be used to accurately predict treatment effects on the clinical end point. Because there are different strengths and weaknesses of the total and chronic slopes, we evaluate both in separate analyses in this paper.

### Measures of Disease Severity

We included three measures of severity of kidney disease that are often targeted in a trial design: baseline GFR, baseline albuminuria, and mean chronic slope in the control arm. The measures of albuminuria varied across studies, with most measuring protein excretion rate. Because guidelines recommend use of urine albumin-to-creatinine ratio (UACR), we express UACR using a commonly used conversion of UACR as 60% of protein excretion rate. For model fitting, we log-transformed UACR to account for positive skewness.

### Trial-Level Analyses

Our analyses extend previous work using meta-regression models that relate treatment effects on the clinical end point to treatment effects on the GFR slope-based surrogate end point across RCTs. The trial-level analysis consists of two steps. In the first step, we used intent-to-treat analyses to estimate the treatment effects on each end point within each trial. We also estimated standard errors and correlations of sampling errors of the estimated effects on the different end points using robust sandwich estimates. In the second step, we fit Bayesian meta-regression models to the treatment effect estimates while accounting for their standard errors and correlations to assess the strength of the association between treatment effects on the separate end points across trials. Four meta-regression parameters are used to interpret surrogate quality: the intercept, slope, meta-regression residual SD (which we refer to as root-mean-squared error [RMSE]), and the coefficient of determination, denoted R². The intercept should be zero, implying a null effect on slope corresponds to a null average effect on the clinical end point. The meta-regression slope should be nonzero, indicating that trials with beneficial (harmful) effects on slope correspond to beneficial (harmful) effects on the clinical end point. Finally, the RMSE should be small relative to the overall SD between studies in the true treatment effects on the clinical end point (corresponding to R² close to 1), indicating that GFR slope can be used to accurately predict the clinical effect.

In this study, we extend the second-stage model to allow meta-regression parameters to vary with severity, which is accomplished by adding interaction terms. Our primary question was whether the meta-regression intercept and/or slope may change with disease severity, reflecting variation in how an effect size on GFR slope translates to an effect size on the clinical end point. Thus, our primary model includes interaction terms for the meta-regression intercept and slope. A nonzero interaction for the intercept indicates that the implications of a null effect on GFR slope differ depending on the level of disease severity. A nonzero interaction for the meta-regression slope indicates that the implications of beneficial (harmful) treatment effects on GFR slope differ depending on disease severity. For our analyses, we centered disease severity data using the mean across trials so that the meta-regression intercept could be interpreted for a trial with the average value defining severity. Strong evidence for effect modification was defined as a 95% credible interval for the interaction terms that excluded zero.

We estimated treatment effects, standard errors, and within-study correlations using SAS version 9.4 and fit the trial-level models using R version 4.0.3, and the RStan package (version 2.21.12) for sampling posterior distributions using Markov Chain Monte Carlo algorithms.

### Prediction Summaries

We summarize posterior predictive distributions for predicted effects on the clinical end point for a hypothetical future trial for a range of treatment effects on the slope-based end points (from a null to a large treatment effect) and values defining CKD severity (for the 25th and 75th percentiles of each measure from the data). These distributions properly account for sampling error in the new trial and uncertainty in the estimated model parameters. For illustration, we use a fixed large trial design (corresponding to roughly 1600 patients), similar to previous work.

### Sensitivity Analyses

We performed sensitivity analyses to assess the robustness of our results. We evaluated results under two models, which relaxed key assumptions made in modeling for our primary analyses: one in which each trial's disease severity measure was regarded as fixed as opposed to being drawn from a common distribution across studies, and the second in which the meta-regression RMSE was allowed to vary with disease severity. We also refit models after removing disease subgroups that stood out because of distinctiveness in their population CKD severity (cardiovascular disease trials because of high baseline GFR and glomerular disease trials because of high baseline UACR), and intervention subgroups with unique mechanisms of action or known extrarenal effects on serum creatinine (immunosuppressant and dietary modification trials). We also refit models allowing interaction with log-transformed mean baseline GFR (instead of with mean baseline GFR itself). Finally, we also evaluated the total slope over 2 years rather than 3 years as the surrogate end point.

---

## Results

Among the 66 trials, there were 186,949 patients and 19,533 (10%) experienced the clinical event (Table 1). Across trials, the mean baseline GFR was 55 (SD ±23) ml/min per 1.73 m², the median baseline UACR was 389 (interquartile range ±894) mg/g, and the median control arm GFR slope was −3.0 (interquartile range ±2.5) ml/min per 1.73 m²/yr.

### Table 1. Summary of trials used for analyses

| Characteristics | Overall | Trials with Low Mean Baseline GFR (<40) | Trials with Moderate Mean Baseline GFR (40–75) | Trials with High Mean Baseline GFR (>75) |
|---|---|---|---|---|
| Patients, N (median) | 186,949 (564) | 14,073 (289) | 51,864 (985) | 121,012 (5519) |
| Clinical events, total (% of patients) | 19,533 (10) | 4601 (33) | 7379 (14) | 7553 (6) |
| Baseline UACR, median (IQR) | 389 (894) | 575 (655) | 643 (1041.9) | 29 (772) |
| Control arm chronic slope, median (IQR) | −3.0 (2.5) | −3.7 (1.8) | −3.6 (2.1) | −1.7 (1.9) |
| **Diseases, total (% of trials)** | | | | |
| Cardiovascular | 7 (11) | 0 (0) | 2 (9) | 5 (23) |
| CKD not otherwise specified | 28 (42) | 19 (86) | 7 (32) | 2 (9) |
| Diabetes | 21 (32) | 2 (9) | 8 (36) | 11 (50) |
| Glomerular | 10 (15) | 1 (5) | 5 (23) | 4 (18) |

(Baseline UACR represented in mg/g; mean control arm chronic slope in ml/min per 1.73 m²/yr. Intervention breakdown includes RASB versus control [21 trials, 32%], immunosuppression [9, 14%], low versus usual BP [7, 11%], SGLT-2 inhibitor [4, 6%], among others.)

Trials with lower GFR typically had higher UACR and faster progression and had higher proportions of patients experiencing the clinical event. Blood pressure modification, RAS blockade, and immunosuppressants were evaluated more frequently than other intervention classes and were evaluated across a broad range of baseline GFR or ACR, and rate of progression. There was less variation across disease severity measures within certain intervention classes. For example, GLP-1 agonists were only evaluated in trials with high baseline GFR and moderate progression rates.

For total slope, there was no evidence that either the meta-regression intercept or slope varied with baseline GFR, UACR, or control arm chronic slope (Figure 1 and Table 2). The 95% credible intervals for the interaction coefficients were narrow and centered near zero in analyses for each disease severity measure. By contrast, for chronic slope, there was strong evidence for variation in both the meta-regression intercept and slope depending on severity (Figure 2 and Table 2). Specifically, these results indicated that the meta-regression slope is larger in magnitude for trials with higher baseline GFR, lower baseline UACR, or slower control arm progression compared with trials with the opposite. We found that the major implications of our results were not substantially changed in any of the sensitivity analyses considered. The results using the 2-year total slope were similar to those obtained using the 3-year total slope, with no strong evidence of interactions.

### Table 2. Meta-regression posterior summaries for continuous interactions models

Posterior medians and 95% credible intervals. (For UACR, interaction coefficients interpreted as multiplicative changes in HRs per two-fold higher UACR; for baseline GFR and control arm slope, as additive changes in log-HRs.)

**Total slope**

| Parameter | Baseline GFR (per 10 ml/min/1.73 m² higher) | Baseline UACR (per two-fold higher, mg/g) | Control arm slope (per 1 ml/min/1.73 m²/yr higher) |
|---|---|---|---|
| Meta-regression intercept at mean severity | −0.05 (−0.11 to 0.01) | −0.05 (−0.12 to 0.01) | −0.06 (−0.13 to −0.003) |
| Meta-regression slope at mean severity | −0.34 (−0.42 to −0.24) | −0.34 (−0.42 to −0.25) | −0.32 (−0.41 to −0.23) |
| Interaction intercept | 0.01 (−0.02 to 0.04) | −0.01 (−0.03 to 0.05) | 0.01 (−0.02 to 0.05) |
| Interaction slope | −0.01 (−0.05 to 0.03) | 0.01 (−0.03 to 0.05) | −0.02 (−0.07 to 0.02) |
| RMSE | 0.06 (0.02 to 0.13) | 0.05 (0.01 to 0.12) | 0.06 (0.02 to 0.13) |
| R² | 0.96 (0.81 to 1.00) | 0.93 (0.77 to 0.99) | 0.94 (0.78 to 0.99) |

**Chronic slope**

| Parameter | Baseline GFR (per 10 ml/min/1.73 m² higher) | Baseline UACR (per two-fold higher, mg/g) | Control arm slope (per 1 ml/min/1.73 m²/yr higher) |
|---|---|---|---|
| Meta-regression intercept at mean severity | −0.03 (−0.13 to 0.06) | −0.09 (−0.21 to 0.02) | −0.08 (−0.20 to 0.05) |
| Meta-regression slope at mean severity | −0.28 (−0.41 to −0.16) | −0.27 (−0.41 to −0.13) | −0.30 (−0.44 to −0.15) |
| Interaction intercept | 0.06 (0.02 to 0.11) ᵃ | −0.09 (−0.16 to −0.03) ᵃ | 0.07 (0.01 to 0.15) ᵃ |
| Interaction slope | −0.08 (−0.16 to −0.003) ᵃ | 0.13 (0.05 to 0.21) ᵃ | −0.10 (−0.18 to −0.03) ᵃ |
| RMSE | 0.16 (0.10 to 0.24) | 0.14 (0.06 to 0.22) | 0.16 (0.09 to 0.24) |
| R² | 0.70 (0.41 to 0.89) | 0.67 (0.40 to 0.85) | 0.68 (0.41 to 0.88) |

ᵃ 95% credible intervals for interaction terms that exclude zero. For interpretation of the RMSE, the total SD for the true treatment effects on the clinical end point has a posterior median (95% CI) of 0.26 (0.19 to 0.36).

Table 3 illustrates the implications for predicted effects on the clinical end point. The predicted HRs for the clinical end point were nearly identical between lower and higher levels of each of the three disease severity measures for prediction using total slope. For example, a treatment effect of 1.5 ml/min per 1.73 m²/yr on the total slope translated to a nearly identical range in predicted HRs (between 0.59 and 0.60) when the mean baseline GFR was 75 to 40 ml/min per 1.73 m². However, there were large changes in the predicted HRs across the same range in severity values when using chronic slope. For example, for a trial with baseline GFR equal to 40 ml/min per 1.73 m², the predicted HR changed from 0.87 if the treatment had no effect on the chronic slope to 0.70 if the treatment had a 1.5 ml/min per 1.73 m²/yr benefit on the chronic slope (a 24% difference). By contrast, for a trial with baseline GFR equal to 75 ml/min per 1.73 m², the predicted HR changed from 1.06 if the treatment had no effect on the chronic slope to 0.61 if the treatment had a 1.5 ml/min per 1.73 m²/yr benefit on the chronic slope (a 74% difference).

### Table 3. Predicted treatment effects on the clinical end point as a function of effects on total or chronic slope and disease severity

Median HR (95% Prediction Interval) at observed treatment effects on GFR slope of 0, 0.75, and 1.5 ml/min/1.73 m²/yr.

**Total slope**

| Disease Severity Level | Effect 0 | Effect 0.75 | Effect 1.5 | % Diff (0 vs 1.5) |
|---|---|---|---|---|
| Low baseline GFR | 0.93 (0.76–1.14) | 0.74 (0.60–0.90) | 0.59 (0.47–0.74) | 58 |
| High baseline GFR | 0.96 (0.78–1.19) | 0.75 (0.60–0.93) | 0.59 (0.47–0.74) | 63 |
| High baseline UACR | 0.92 (0.75–1.13) | 0.75 (0.61–0.90) | 0.59 (0.47–0.72) | 56 |
| Low baseline UACR | 0.95 (0.77–1.16) | 0.74 (0.60–0.89) | 0.59 (0.47–0.72) | 61 |
| Fast GFR progression | 0.91 (0.74–1.13) | 0.74 (0.60–0.90) | 0.60 (0.48–0.74) | 52 |
| Slow GFR progression | 0.96 (0.77–1.18) | 0.75 (0.60–0.92) | 0.59 (0.46–0.73) | 63 |

**Chronic slope**

| Disease Severity Level | Effect 0 | Effect 0.75 | Effect 1.5 | % Diff (0 vs 1.5) |
|---|---|---|---|---|
| Low baseline GFR | 0.87 (0.60–1.26) | 0.78 (0.54–1.11) | 0.70 (0.47–1.02) | 24 |
| High baseline GFR | 1.06 (0.71–1.60) | 0.81 (0.54–1.20) | 0.61 (0.39–0.93) | 74 |
| High baseline UACR | 0.81 (0.58–1.14) | 0.75 (0.53–1.07) | 0.70 (0.49–0.94) | 16 |
| Low baseline UACR | 0.98 (0.69–1.41) | 0.75 (0.55–1.01) | 0.58 (0.39–0.83) | 69 |
| Fast GFR progression | 0.84 (0.57–1.23) | 0.74 (0.52–1.05) | 0.66 (0.45–0.93) | 27 |
| Slow GFR progression | 1.02 (0.69–1.53) | 0.78 (0.51–1.14) | 0.58 (0.37–0.88) | 76 |

Severity definitions: Low baseline GFR: 40 ml/min/1.73 m²; high baseline GFR: 75; low baseline UACR: 71 mg/g; high baseline UACR: 1000 mg/g; fast GFR progression: −4.0 ml/min/1.73 m²/yr; slow GFR progression: −1.5 ml/min/1.73 m²/yr. This table highlights that differences in predicted HRs for treatment effects on the clinical end point can vary considerably more across the range of treatment effects on slope when chronic slope is used than when total slope is used.

---

## Discussion

This article extends prior work evaluating GFR slope. We assessed whether the relationship between treatment effects on slope and treatment effects on an established clinical end point differs depending on the severity of CKD in the study population. We considered three metrics for severity: baseline GFR, UACR, and control arm GFR slope. We found the association of effects on 3-year total slope with effects on the clinical end point consistent across measures of patient population disease severity. By contrast, we found variation by disease severity in the association when evaluating chronic slope. Our analyses showed that treatment effects on chronic slope translated to progressively larger treatment effects on the clinical end point for patient populations with less as opposed to more severe disease. These results can aid in interpreting treatment effects on slope-based end points in ongoing and future trials.

As described in a separate study using the same 66 trials, treatment effects on the 3-year total slope predict treatment effects on the clinical end point with greater accuracy than using chronic slope. The results of this study suggest that this greater accuracy may be explained, in part, by a greater stability in the trial-level association of the total versus chronic slope across measures of CKD severity. The explanation for why severity influences the trial-level association for chronic slope, but not for the total slope, is not completely clear. One possible explanation arises from the relationship between acute effects and treatment effects on chronic slope. Glomerular hyperfiltration is a common pathway underlying CKD progression. Reducing glomerular hyperfiltration with dietary or pharmacological interventions can result in a negative acute effect on GFR in the short term, but in the long term, such interventions can stabilize GFR, as reflected by the chronic slope. This mechanism may lead to a negative correlation between the effect on the acute GFR slope and the effect on the chronic slope, in which case the clinical benefit of slowing decline in the chronic slope may be partially offset by the clinical implications of greater acute declines in GFR. Some have suggested that the inverse association between acute and chronic effects may be stronger for patients with more advanced disease. As such, it is possible that treatment benefits on the chronic slope would be counteracted by the negative acute effects to a greater degree in studies of patients with more advanced disease compared with less advanced disease. Such a pattern could potentially explain the observed attenuation of the hazard reduction associated with a given effect on the chronic slope with more severe disease. Alternatively, because the treatment effect on total slope incorporates the acute effect, effects on the total slope would remain weaker than effects on the chronic slope for studies with larger negative acute effects, mitigating the tendency for apparent strongly beneficial slope-based effects in studies with severe CKD.

Our finding of an association between CKD severity and how treatment effects on the chronic slope (expressed on the absolute scale) relate to treatment effects on the clinical end point (expressed on the relative scale) can be seen as analogous to findings reported in other medical domains. For example, across a collection of trials for heart failure, stroke, and other diseases, Kent et al. found heterogeneity in treatment effect sizes across quartiles defined by baseline disease risk for effects represented as absolute risk differences, but less so for effects represented as relative risk differences. These authors noted that the relationship between treatment effects expressed as absolute and relative differences can often be predicted by disease severity as measured by the absolute risk of the outcome. There are important reasons why we use absolute (mean differences) as opposed to relative differences (a ratio) for treatment effects on GFR slope. In general, a ratio of means can be an unstable quantity to estimate when the numerator and denominator can be positive or negative, and especially when the denominator (estimated mean control arm slope) can be close to zero.

A major implication of this study is that the relationship between treatment effects on total slope and those of the clinical end point appears consistent across levels of disease severity. These results suggest that the overall meta-regression model for 3-year total slope can be used to predict treatment effects on the clinical end point across the range of patient population disease severity. On the other hand, our results indicate that disease severity should be considered when translating the magnitude of a treatment effect on chronic slope to the magnitude of the projected treatment effect on the clinical end point. Our results did show that the predicted HRs are relatively consistent across levels of disease severity for effects on chronic slope near 0.75 ml/min per 1.73 m²/yr. However, the validity of a surrogate end point relies on consistent interpretation across the full spectrum of effect sizes, from that of the null hypothesis to a large treatment benefit. Finally, although we found no evidence that the prediction accuracy on the basis of the total slope (expressed as the RMSE) varies with disease severity, there was a trend to suggest the chronic slope might be used to more accurately predict effects on the clinical end point in trials with more compared with less severe disease.

### Strengths and Limitations

There are several strengths to the analyses reported. We obtained individual participant data from 66 well-powered RCTs. The abundance of high-quality data enabled us to use more intricate models than typically possible in surrogate evaluations. Use of individual-level data allowed us to appropriately account for multiple sources of variation in the treatment effect estimates and enabled us to evaluate the influence of three measures of disease severity. Having multiple measures helped us corroborate results from separate analyses. By using Bayesian modeling, we were able to report probability for treatment effects in hypothetical future trials, which improved the interpretability and intuition behind our results.

There are also several limitations. First, disease severity is multifaceted and associated with distinct intervention options. We did not attempt to identify the causal mechanism behind the interactions observed. We also did not attempt to evaluate if our results persisted within all subgroups of trials defined by specific disease conditions or specific interventions, as statistical power for evaluating interactions within many subgroups is very low. We did observe that the results of our analyses were not substantially changed after removing subsets of trials whose populations or treatments exhibited unique characteristics. It is possible that the clinical implications of the disease severity indices may differ between the earlier and later trials included in our analyses because of improvements in standards of care. We used a guideline-recommended method to convert urine protein to UACR; however, this may vary by disease and other population characteristics. These analyses were also limited by use of clinical events acquired only over the duration of the trial as the reference standard, but this is a common challenge to surrogate end point evaluation using previously conducted trials. Finally, our calculation for the total slope over 3 years requires an extrapolation of the data for trials with <3 years of follow-up. However, treatment effects on 3-year GFR slope defined this way have been found to predict treatment effects on the clinical end point with high accuracy, and this work further corroborates this result.

Overall, the analyses reported help improve understanding of how to interpret treatment effects on GFR slope-based end points in RCTs. Our results indicate the general interpretability and applicability of the trial-level association for the total slope, which is consistent across levels of disease severity in the patient population. However, our results indicate that treatment effects on chronic slope should be interpreted in the context of population disease severity. Future work should continue to refine optimal trial design strategies for trials on the basis of CKD severity.

---

## Funding

The study was funded by the National Kidney Foundation (NKF). NKF has received consortium support from AstraZeneca, Bayer, Cerium, Chinook, Boehringer Ingelheim, CSL Behring, Novartis, and Travere. A variety of sources have supported the RCTs included in the CKD-EPI CT. This work received support from the Utah Study Design and Biostatistics Center, with funding in part from the National Center for Advancing Translational Sciences of the NIH under Award Number UL1TR002538.

---

## Key References

1. Inker LA, Heerspink HJL, Tighiouart H, et al. GFR slope as a surrogate end point for kidney disease progression in clinical trials: a meta-analysis of treatment effects of randomized controlled trials. J Am Soc Nephrol. 2019;30(9):1735-1745. doi:10.1681/ASN.2019010007
2. Levey AS, Inker LA, Matsushita K, et al. GFR decline as an end point for clinical trials in CKD: a scientific workshop sponsored by the NKF and the US FDA. Am J Kidney Dis. 2014;64(6):821-835. doi:10.1053/j.ajkd.2014.07.030
3. Grams ME, Sang Y, Ballew SH, et al. Evaluating glomerular filtration rate slope as a surrogate end point for ESKD in clinical trials: an individual participant meta-analysis of observational data. J Am Soc Nephrol. 2019;30(9):1746-1755. doi:10.1681/ASN.2019010008
4. Greene T, Ying J, Vonesh EF, et al. Performance of GFR slope as a surrogate endpoint for kidney disease progression in clinical trials: a statistical simulation. J Am Soc Nephrol. 2019;30(9):1756-1769. doi:10.1681/ASN.2019010009
7. Vonesh E, Tighiouart H, Ying J, et al. Mixed-effects models for slope-based endpoints in clinical trials of chronic kidney disease. Stat Med. 2019;38(22):4218-4239. doi:10.1002/sim.8282
15. Kent DM, Nelson J, Dahabreh IJ, Rothwell PM, Altman DG, Hayward RA. Risk and treatment effect heterogeneity: re-analysis of individual participant data from 32 large clinical trials. Int J Epidemiol. 2016;45(6):2075-2088. doi:10.1093/ije/dyw118
18. Neuen BL, Tighiouart H, Heerspink HJL, et al. Acute treatment effects on GFR in randomized clinical trials of kidney disease progression. J Am Soc Nephrol. 2022;33(2):291-303. doi:10.1681/ASN.2021070948
19. Inker LA, Collier W, Heerspink HJL, et al. GFR slope as a surrogate end point for kidney failure in clinical trials: an updated meta-analysis of treatment effects of randomized controlled trials. (In preparation.)

*Received: August 12, 2022. Accepted: December 2, 2022.*
