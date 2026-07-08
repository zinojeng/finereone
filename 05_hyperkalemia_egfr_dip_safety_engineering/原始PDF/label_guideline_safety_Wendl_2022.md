---
title: "Physiologically-based pharmacokinetic modeling to predict CYP3A4-mediated drug-drug interactions of finerenone"
authors: "Wendl T; Frechen S; Gerisch M; Heinig R; Eissing T"
year: 2022
journal: "CPT: Pharmacometrics & Systems Pharmacology"
doi: "10.1002/psp4.12746"
pmid: "34783193"
source: "Europe PMC (open access; CC BY-NC), PMID 34783193"
volume: "11(2):199-211"
verified: true
---

# Physiologically-based pharmacokinetic modeling to predict CYP3A4-mediated drug-drug interactions of finerenone

**Authors:** Thomas Wendl¹, Sebastian Frechen¹, Michael Gerisch²,³, Roland Heinig³, Thomas Eissing¹

¹ Pharmaceuticals R&D, Pharmacometrics, Bayer AG, Leverkusen, Germany
² Pharmaceuticals R&D, Drug Metabolism and Pharmacokinetics, Bayer AG, Wuppertal, Germany
³ Pharmaceuticals R&D, Clinical Pharmacology, Bayer AG, Wuppertal, Germany

**Correspondence:** Thomas Eissing, Bayer AG, Pharmaceuticals R&D, Pharmacometrics, Building B106 Room 205, 51368 Leverkusen, Germany. Email: thomas.eissing@bayer.com

**Funding:** No funding was received for this work.

Received 8 August 2021; Revised 29 September 2021; Accepted 31 October 2021.
© 2021 Bayer AG. CPT: Pharmacometrics & Systems Pharmacology published by Wiley Periodicals LLC on behalf of the American Society for Clinical Pharmacology and Therapeutics. Open access under Creative Commons Attribution-NonCommercial License.

DOI: 10.1002/psp4.12746 — CPT Pharmacometrics Syst Pharmacol. 2022;11:199–211.

---

## Abstract

Finerenone is a nonsteroidal, selective mineralocorticoid receptor antagonist that recently demonstrated its efficacy to delay chronic kidney disease (CKD) progression and reduce cardiovascular events in patients with CKD and type 2 diabetes. Here, we report the development of a physiologically-based pharmacokinetic (PBPK) model for finerenone and its application as a victim drug of cytochrome P450 3A4 (CYP3A4)-mediated drug-drug interactions (DDIs) using the open-source PBPK platform PK-Sim, which has recently been qualified for this application purpose.

First, the PBPK model for finerenone was developed using physicochemical, in vitro, and clinical (including mass balance) data. Subsequently, the finerenone model was validated regarding the contribution of CYP3A4 metabolism to total clearance by comparing with observed data from dedicated clinical interaction studies with:
- **Erythromycin**: simulated geometric mean ratios of the area under the plasma concentration-time curve (AUCR) of **3.46** and geometric mean peak plasma concentration ratios (Cmax R) of **2.00** vs. observed of **3.48** and **1.88**, respectively.
- **Verapamil**: simulated AUCR of **2.91** and Cmax R of **1.86** vs. observed of **2.70** and **2.22**, respectively.

Finally, the finerenone model was applied to predict clinically untested DDI studies with various CYP3A4 modulators:
- **Itraconazole**: AUCR **6.31**, Cmax R **2.37**
- **Clarithromycin**: AUCR **5.28**, Cmax R **2.25**
- **Cimetidine**: AUCR **1.59**, Cmax R **1.40**
- **Fluvoxamine**: AUCR **1.57**, Cmax R **1.38**
- **Efavirenz**: AUCR **0.19**, Cmax R **0.32**
- **Rifampicin**: AUCR **0.07**, Cmax R **0.14**

This PBPK analysis provides a quantitative basis to guide the label and clinical use of finerenone with concomitant CYP3A4 modulators.

## Study Highlights

**What is the current knowledge on the topic?**
Kerendia (finerenone), a novel drug indicated in chronic kidney disease with type 2 diabetes, is a sensitive CYP3A4 substrate. It was tested with the moderate CYP3A4 inhibitors erythromycin and verapamil in clinical DDI studies influencing the pharmacokinetics (PKs) of finerenone.

**What question did this study address?**
What effects predict PBPK models for clinically untested CYP3A4 modulators on the finerenone PKs?

**What does this study add to our knowledge?**
This study complements the finerenone-drug interaction program informing scientists and prescribers as well as the drug label about the expected extent of CYP3A4 interactions on the finerenone PKs for inhibitors and inducers not tested clinically.

**How might this change drug discovery, development, and/or therapeutics?**
This PBPK model-based DDI assessment applied a qualified CYP3A4 compound network approach using the open-source systems pharmacology platform (PK-Sim). As strong inhibitors and inducers were not studied clinically, such strong modulators did not provide the boundaries for interpolation to less sensitive DDI scenarios ("classical approach"), but were part of the prediction and thus extrapolated.

---

## Introduction

Finerenone (Kerendia) is a nonsteroidal, selective mineralocorticoid receptor antagonist that demonstrated efficacy to delay progression of kidney disease and reduce cardiovascular events in patients with CKD and type 2 diabetes in the pivotal outcome trial **FIDELIO-DKD (NCT02540993)**.

The clinical pharmacology program for finerenone comprises 27 phase I studies to date. The PKs of finerenone are dose-linear across the entire range of investigated doses (**1.25 to 80 mg**). Following oral administration, finerenone is rapidly and completely absorbed. It is eliminated almost exclusively by CYP3A4 metabolism and to a much smaller extent by CYP2C8. Finerenone also shows a relevant first pass CYP3A4-mediated metabolism in the gut wall and the liver.

- Absolute bioavailability after oral administration: **43.5%**
- Hepatic bioavailability: **0.756**
- Fraction escaping gut wall metabolism (Fg): **0.575**
- ~42% of orally administered finerenone metabolized during first pass in gut wall
- All formed major plasma metabolites are pharmacologically inactive
- ~1% of dose renally eliminated unchanged by glomerular filtration
- Plasma protein binding: moderate (~92%)

## Methods

### Finerenone PBPK model development

The PBPK model was informed with physicochemical data, clinical data (including mass balance), absolute bioavailability (BA) study data, multiple dose escalation study, and a gemfibrozil DDI study. The final PBPK model comprises metabolization via CYP3A4 and CYP2C8 and renal excretion via glomerular filtration.

A weak irreversible inhibition on CYP3A4 was observed in vitro and, although negligible, was included as a mechanism-based CYP3A4 (auto-)inactivation.

The CYP2C8 pathway contribution was informed via an interaction study with the strong CYP2C8 inhibitor **gemfibrozil**. In this clinical study, an AUCR of **1.10** was observed for finerenone under gemfibrozil (600 mg twice daily) co-administration. Assuming complete inhibition of CYP2C8:
- hepatic fm_CYP3A4 = 1/AUCR = **0.908**
- fm_CYP2C8,hep = 1 − fm_CYP3A4,hep = **0.092**
- Remaining hepatic metabolic clearance assumed solely CYP3A4-mediated, contributing ~90% in the final model.

The finerenone PK-Sim files are provided on https://github.com/Open-Systems-Pharmacology/Finerenone-Model.

### Virtual populations

Virtual phase I populations created with the "PKSimCreatePopulation" algorithm (OSP Matlab toolbox); populations of 1000 individuals, ages 18 to 45 years.

### Validation of finerenone model as a CYP3A4 victim

CYP3A4 contribution validated using:
- **Erythromycin** (500 mg t.i.d., moderate CYP3A4 inhibitor): observed finerenone AUCR **3.48** and Cmax R **1.88**
- **Verapamil** (240 mg o.d., moderate CYP3A4 inhibitor and P-gp inhibitor): observed finerenone AUCR **2.70** and Cmax R **2.22**

No parameters were modified or adjusted to simulate the virtual phase I population.

### Prediction of clinically untested DDI scenarios

Modulators predicted:
- **Itraconazole** — strong index inhibitor
- **Clarithromycin** — strong index inhibitor
- **Fluvoxamine** — moderate inhibitor (classified as weak inhibitor until 2019)
- **Cimetidine** — weak inhibitor
- **Rifampicin** — strong inducer
- **Efavirenz** — moderate inducer

Classification per FDA website on Drug Interactions (Tables of Substrates, Inhibitors, and Inducers).

### Sensitivity analysis

Contributions of CYP3A4 and CYP2C8 to hepatic metabolic clearance were adjusted:
- **Reference scenario**: hepatic fm_CYP3A4 ~0.90 / fm_CYP2C8 ~0.10
- **Scenario #1**: fm_CYP3A4 ~0.85 / fm_CYP2C8 ~0.15
- **Scenario #2**: fm_CYP3A4 ~0.95 / fm_CYP2C8 ~0.05

### Software

PK-Sim and MoBi, Open Systems Pharmacology Suite (OSPS version 9.1.3); Matlab R2017b. Perpetrator models validated for DDI simulations by the OSP community.

## Results

### Model development and validation

Simulated concentration-time profiles of the virtual phase I population showed good agreement with observed data over a variety of doses and dosing schedules.

- Simulated AUCR with erythromycin (500 mg t.i.d.): **3.46** (in line with observed **3.48**); simulated Cmax R **2.00** (observed **1.88**)
- Simulated AUCR with verapamil (120/240 mg o.d.): **2.91** (observed **2.70**); simulated Cmax R **1.86** (observed **2.22**)
- All simulated values fall within 80–125% of observed values.

### Prediction of clinically untested DDI scenarios

Predicted AUCR and Cmax R values (geo. mean; geo. CV) — from Figure 4:

| Modulator | Dose | AUCR (geo. mean) | Cmax R (geo. mean) |
|---|---|---|---|
| Itraconazole | 200 mg BID | 6.31 | 2.37 |
| Clarithromycin | 500 mg BID | 5.28 | 2.25 |
| Erythromycin (observed) | 500 mg TID | 3.48 | 1.88 |
| Erythromycin (simulated) | 500 mg TID | 3.46 | 2.00 |
| Verapamil (simulated) | 120/240 mg | 2.91 | 1.86 |
| Verapamil (observed) | 120/240 mg | 2.70 | 2.22 |
| Cimetidine | 800 mg BID | 1.59 | 1.40 |
| Fluvoxamine | 100 mg BID | 1.57 | 1.38 |
| Efavirenz | 400 mg OD | 0.20 | 0.34 |
| Efavirenz | 600 mg OD | 0.19 | 0.32 |
| Rifampicin | 600 mg OD | 0.07 | 0.14 |

### Sensitivity analysis (Table 1 — three scenarios)

| Modulator | Scenario | AUCR geo. mean | Cmax R geo. mean |
|---|---|---|---|
| Erythromycin | Observed | 3.48 | 1.88 |
| | Reference | 3.46 | 2.00 |
| | #1 | 3.19 | 1.93 |
| | #2 | 3.74 | 2.07 |
| Verapamil | Observed | 2.70 | 2.22 |
| | Reference | 2.91 | 1.86 |
| | #1 | 2.73 | 1.80 |
| | #2 | 3.09 | 1.91 |
| Gemfibrozil | Observed | 1.10 | 1.16 |
| | Reference | 1.11 | 1.06 |
| Itraconazole | Reference | 6.31 | 2.37 |
| | #1 | 5.23 | 2.24 |
| | #2 | 7.76 | 2.50 |
| Clarithromycin | Reference | 5.28 | 2.25 |
| | #1 | 4.52 | 2.14 |
| | #2 | 6.27 | 2.36 |
| Fluvoxamine | Reference | 1.57 | 1.38 |
| Cimetidine | Reference | 1.59 | 1.40 |
| Efavirenz | Reference | 0.19 | 0.32 |
| Rifampicin | Reference | 0.071 | 0.14 |

The reference scenario (fm_CYP3A4 ~0.90) best described the evaluated interactions. Differences among the three scenarios were small.

## Discussion

The total fm_CYP3A4 (of total clearance) in the finerenone PBPK model is ~**0.93** (0.42 in gut wall and 0.51 in liver). This is consistent with fm_CYP3A4 estimations reported by Heinig et al. (point estimates 0.88 and 0.89 for erythromycin- and verapamil-based static calculations). Propagating the reported 90% confidence intervals translates to a fm_CYP3A4 range of **0.83 to 0.94**.

Mechanism-based auto-inactivation by finerenone occurs in both liver and intestine but its impact is low. The finerenone linearity factor R_lin (AUC_0-24,day10 / AUC_inf,day1) was ≤1.32 and the AUCR for midazolam was ≤1.21, indicating a very small perpetrator effect (reduction in active CYP3A4 enzyme by ~0.4% in liver; up to 40% in steady-state intestine).

Predicted AUCR values for finerenone combinations fall within published observed ranges for other sensitive CYP3A4 victim drugs (midazolam, triazolam, alprazolam, alfentanil). For efavirenz (600 mg), predicted AUCR of 0.19 comparable to alfentanil observed values, classified as strong induction per FDA; 400 mg efavirenz gave AUCR slightly higher than 0.20 (moderate induction).

Geometric mean fold error (GMFE) of the CYP3A4-DDI network on OSP was ~1.39 on AUC and 1.37 on Cmax:
- Competitive inhibition combinations (itraconazole, cimetidine, fluvoxamine): GMFE AUCR 1.49, Cmax R 1.27
- MBI combinations (clarithromycin, erythromycin, verapamil): GMFE AUCR 1.27, Cmax R 1.24
- Inducers (efavirenz, rifampicin): GMFE AUCR 1.38, Cmax R 1.48

### Clinical / labeling implications

- FIDELIO-DKD: finerenone approved by FDA with dosing guidance including monitoring and dose adjustment. 10 or 20 mg OD administered based on serum potassium and eGFR.
- Serum potassium-based dose titration highlighted as important context for CYP3A4 inhibitor label guidance.
- **Strong CYP3A4 inhibitors are contraindicated.**
- For **moderate or weak CYP3A4 inhibitors**, recommended to monitor serum potassium during drug initiation or dosage adjustment of either finerenone or the CYP3A4 inhibitor, and adjust finerenone dosage as appropriate.
- **Concomitant use of strong or moderate CYP3A4 inducers should be avoided.**

The presented PBPK analyses of finerenone as victim of CYP3A4-mediated DDI can be considered in lieu of clinical DDI study-based data for modulator categories lacking such studies, as reflected in the USPI under "Drug Interaction Studies - Clinical Studies and Model-Informed Approaches."

## Conflict of Interest

T.W., S.F., M.G., R.H., and T.E. are Bayer employees and potential shareholders of Bayer AG. T.W. and S.F. use Open Systems Pharmacology software, tools, or models in their professional roles. S.F. is a member of the Open-Systems-Pharmacology Sounding Board.

---

*Full text (13 pages) retrieved and visually verified from Europe PMC PDF (PMID 34783193). Title, authorship, journal, DOI, and numeric values confirmed against publisher record. Numeric DDI values (AUCR, Cmax R) transcribed from Figure 4 and Table 1.*
