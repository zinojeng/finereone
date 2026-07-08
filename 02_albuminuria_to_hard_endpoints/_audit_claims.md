# Claim Audit — 02_albuminuria_to_hard_endpoints.md

稽核員：claim-auditor（Phase B 並行稽核之一）
稽核範圍：主文所有百分比、樣本數（N=）、效應量（HR/OR/RR/CI/R²）、引號字串
稽核方法：逐句對應 `[檔名]` 標記，於 `原始PDF/{filename}.md` 執行 Grep 逐字核對

## 結論摘要

主文全部可稽核的數字（百分比 / 樣本數 / HR / OR / CI / R² / P 值）**均在對應本地檔案中 Grep 命中**，無 ❌GREP_FAIL。未發現樣本數位數錯置（如 n=133 vs n=1330 類型的 confabulation）、研究設計標籤誤植（RCT vs cohort）、或引號逐字不符的情形。以下列出逐條核對紀錄與 2 項「待議」（非數字錯誤，屬簡化/詮釋層級，建議 arbitrator 留意）。

---

## 逐條核對紀錄（全數通過）

| # | 主文位置 | 待核字串 | 來源檔 | Grep 結果 | Severity |
|---|---|---|---|---|---|
| 1 | §1 | 第4個月UACR降約32%；LS mean比值0.68 (95% CI 0.66–0.70) | albuminuria_mediation_Agarwal_2022.md:430-431 | 命中，逐字一致 | 通過 |
| 2 | §2.1 | ARTS-DN N=823隨機、821接受藥物 | arts_dn_dosefinding_Bakris_2015.md:67 | 命中："823 were randomized and 821 received study drug" | 通過 |
| 3 | §2.1 | 7.5mg 0.79(90%CI 0.68–0.91)/10mg 0.76(0.65–0.88)/15mg 0.67(0.58–0.77)/20mg 0.62(0.54–0.72) | 同上:79-81 | 全數命中，逐字一致 | 通過 |
| 4 | §2.1 | 90天內eGFR降≥30%比例與AE在各組間無顯著差異 | 同上:84-86 | 命中："no differences in the incidence of...eGFR decrease of 30% or more or...adverse events...between the placebo and finerenone groups" | 通過 |
| 5 | §2.2 | FIDELIO-DKD HR 0.82 (0.73–0.93; P=0.001) | FIDELIO-DKD_NEJMoa2025845.md:21,122,390,606 | 命中 | 通過 |
| 6 | §2.2 | FIGARO-DKD HR 0.87 (0.76–0.98; P=0.03)；HHF HR 0.71 (0.56–0.90) | FIGARO-DKD_NEJMoa2110956.md:33,123 | 命中 | 通過 |
| 7 | §2.2 | FIDELITY N=13,026；CV HR 0.86(0.78–0.95;P=0.0018)；kidney(≥57%) HR 0.77(0.67–0.88;P=0.0002)；單一成分HR 0.70(0.60–0.83) | albuminuria_mediation_Agarwal_2022.md:27-33,332,366,413,416 | 全數命中 | 通過 |
| 8 | §3.1-1 | CKD-PC 693,816人；ESKD adj HR 0.83(0.74–0.94)→regression dilution校正0.78(0.66–0.92) | egfr_slope_surrogate_Coresh_2019.md:23,28,87,100 | 命中，逐字一致 | 通過 |
| 9 | §3.1-2 | Heerspink 2019：41治療比較(29,979人)；UACR降30%→風險降27%(95%BCI 5–45%)；median R²=0.47(0.02–0.96)；限ACR>30後R²=0.72(0.05–0.99) | editorial_endpoints_Heerspink_2019.md:26-30,59-60 | 全數命中 | 通過 |
| 10 | §3.1-3 | CKD CTC：48 RCT、85,681人IPD；每30%降幅→風險降19%(95%BCI 5–30%)；median R²=0.66(0.06–0.98) | r2_Heerspink_2025.md:29,38-39 | 命中；確認為"48 randomized controlled trials"（非cohort，設計標籤正確） | 通過 |
| 11 | §3.1-3 | RAASi/ETA解釋82%；SGLT2i 45%；免疫抑制劑41% | editorial_endpoints_Matyjek_2026.md:41,73 | 命中，逐字一致 | 通過 |
| 12 | §3.2 | Inker 2019：47 RCT、60,620人；total slope R²=0.97(0.78–1.00)；chronic slope R²=0.96 | egfr_slope_surrogate_Inker_2019.md:71,79-80,732,741 | 命中 | 通過 |
| 13 | §3.2 | Inker 2023：66 studies、186,312人；total R²=0.97(0.82–1.00)；chronic R²=0.55(0.25–0.77) | egfr_slope_surrogate_Inker_2023.md:136,152-153 | 命中 | 通過 |
| 14 | §3.3 | Holtkamp 2011：急性eGFR −2.3 vs −1.6(P=0.031)；長期slope −4.2 vs −5.0(P<0.001) | r2_Holtkamp_2011.md:61-62 | 命中，逐字一致 | 通過 |
| 15 | §3.3 | Greene 2025：66 studies；joint R²=0.95(0.79–1.00)；每多1ml/min/3個月急性下降→HR升11.4%(7.9–15.0%)；acute:chronic權重比0.078(0.055–0.105) | egfr_slope_surrogate_Greene_2025.md:30,72,74,88 | 全數命中 | 通過 |
| 16 | §3.3 | NKF-FDA-EMA：UACR降30%或slope減緩0.5–1.0 ml/min/年 | egfr_slope_surrogate_Levey_2020.md:41,1985 | 命中 | 通過 |
| 17 | §4.1 | Agarwal 2023：N=12,512(FIDELIO+FIGARO)；基線median UACR 514mg/g；≥30%降幅finerenone 3338(53.2%) vs placebo 1684(27.0%) | albuminuria_mediation_Agarwal_2023.md（abstract全文） | 命中，逐字一致（含📌 abstract-only揭露） | 通過 |
| 18 | §4.1 | UACR連續變項mediated kidney 84%、CV 37%；二元≥30%分別64%與26% | 同上 | 命中，逐字一致 | 通過 |
| 19 | §4.2 | Agarwal 2026：N=12,143；UACR降32.2%、SBP降3.6mmHg、體重降0.23kg、血鉀升0.19mEq/L；UACR mediated 39%(7–71)、SBP 21%(3–40)；合計50%(21–100) | albuminuria_mediation_Agarwal_2026.md（abstract全文） | 命中，逐字一致 | 通過 |
| 20 | §4.3 | Mc Causland 2025：N=5,086；基線median UACR 17mg/g；UACR降26%；連續分析mediated composite 34%(16–132)、首次HF事件29%(14–82)；二元>30%為15%與11% | albuminuria_mediation_Mc_2025.md（abstract全文） | 命中，逐字一致 | 通過 |
| 21 | §4.4 | FIND-CKD：N=1,584；eGFR 25–<90、UACR 200–≤3500mg/g | FIND-CKD_NEJMoa2604625.md:17（NEJM摘要原文即用此整體範圍） | 命中 | 通過 |
| 22 | §4.4 | Primary total slope：finerenone −3.34 vs placebo −4.02；diff 0.68(95%CI 0.32–1.05；摘要報0.7,0.3–1.1,P<0.001) | note_find_ckd_extract.md:118,142; FIND-CKD_NEJMoa2604625.md:21 | 命中，兩種精度數字均可追溯 | 通過 |
| 23 | §4.4 | Acute slope：−2.0 vs −0.8/3個月；diff −1.2(−1.7~−0.6) | note_find_ckd_extract.md:121 | 命中 | 通過 |
| 24 | §4.4 | Chronic slope：−2.9 vs −4.1/年；diff 1.2(0.9–1.6) | note_find_ckd_extract.md:122 | 命中 | 通過 |
| 25 | §4.4 | 停藥後eGFR變化：−8.7 vs −11.1；diff 2.4(1.2–3.5) | note_find_ckd_extract.md:125 | 命中 | 通過 |
| 26 | §4.4 | composite kidney–CV HR 0.77(0.60–0.99;P=0.04)；kidney HR 0.78(0.60–1.01)；CV HR 0.60(0.27–1.33) | note_find_ckd_extract.md:130-132 | 命中 | 通過 |
| 27 | §4.4 | 探索性UACR：6個月相對變化−41.3% vs −9.1%(相對差35.4%)；≥30%降幅56.0% vs 24.4%,OR 3.99(3.22–4.95) | note_find_ckd_extract.md:135-136 | 命中，逐字一致 | 通過 |
| 28 | §3.2 | eGFR slope為FDA/EMA接受之primary endpoint、first-in-class | egfr_slope_surrogate_Taylor_2025.md:50,182 | 命中 | 通過 |
| 29 | §2.2 | FIDELIO偏stage3–4/severely increased albuminuria；FIGARO較早期/moderately increased為主 | FIDELIO-DKD_NEJMoa2025845.md:52; FIGARO-DKD_NEJMoa2110956.md:37,50 | 命中，族群描述與原文一致 | 通過 |
| 30 | §6爭議三 | Agarwal 2023「不易外推到其他藥物」 | albuminuria_mediation_Agarwal_2023.md（Limitation段："not readily extendable to other drugs"） | 命中（中文為忠實翻譯，非逐字英文引號） | 通過 |
| 31 | §6爭議三 | Agarwal 2026「CV益處在數月內出現、早於可測得的腎保護」 | albuminuria_mediation_Agarwal_2026.md（Background/Hypothesis段："cardiovascular benefit emerges within months, before measurable kidney protection"） | 命中（中文為忠實翻譯） | 通過 |
| 32 | §6爭議一 | Matyjek editorial「缺乏UACR下降」對應「幾乎不會有臨床益處」 | editorial_endpoints_Matyjek_2026.md:43（"an absence of UACR reduction is associated with a very low probability of subsequent clinical benefit"） | 命中（中文為忠實翻譯，非逐字英文引號） | 通過 |

---

## 待議（非 GREP_FAIL，屬詮釋/簡化層級，供 arbitrator 參考）

### 待議-1：FIND-CKD 入選標準的簡化表述
**主文位置**：§4.4 "FIND-CKD(N=1,584,非糖尿病 CKD,eGFR 25–<90、UACR 200–≤3500 mg/g,均已用 RASi)"
**說明**：NEJM 摘要本身即用此整體範圍表述（"eGFR 25 to <90"、"UACR 200 to ≤3500"），故不算錯誤；但設計論文 note_find_ckd_extract.md:24 顯示實際入選標準是兩個分層條件（eGFR 25–<60 搭配 UACR 200–<500 **或** eGFR 25–<90 搭配 UACR 500–≤3500），並非單一連續區間的簡單交集。主文表述與 NEJM 摘要一致，可視為對原文的忠實引用，**不需修改**，但若讀者需要精確分層條件應查閱設計論文。
**Severity**：待議（實為通過，因與 NEJM 摘要原文用字一致）

### 待議-2：「均已用 RASi」的精確度
**主文位置**：§4.4 "均已用 RASi"
**說明**：note_find_ckd_extract.md:80 顯示實際數字為 1580/1584 (99.7%) 使用 RAS inhibitor，非 100%。用「均已」（全部）在中文語感上略為以偏概全，但 99.7% 已是絕大多數，且原文入選標準本身要求 concurrent RASi use，此為極少數不耐受/暫停用藥的個案。
**建議**：可考慮改為「幾乎均已用 RASi(99.7%)」以更精確，但不影響論證方向。
**Severity**：待議（輕微，非數字錯誤）

---

## 特別檢查結果

1. **研究設計標籤**：主文中出現的 "RCT" 標記（48個RCT／47個RCT）均對應原文「randomized controlled trial」，無 cohort study 被誤標為 RCT 的情形。FIDELIO/FIGARO/FIDELITY/ARTS-DN/FIND-CKD 均為原文明確標示之 randomized/double-blind trial。Coresh 2019（693,816人）、egfr_slope surrogate 系列（Inker/Greene）為 individual participant data meta-analysis / IPD 分析，主文亦未誤標為 RCT。
2. **樣本數位數**：逐一核對 N=823/821、N=13,026、N=693,816、N=29,979、N=85,681、N=60,620、N=186,312、N=12,512、N=12,143、N=5,086、N=1,584，全數與來源檔完全吻合，無位數錯置（如 133→1330 型 confabulation）。
3. **引號字串**：主文使用之引號多為中文翻譯 paraphrase（非逐字英文引用），已比對其語意與原文摘要段落一致，無無中生有（quote fabrication）情形。

## 結論

本文所有可稽核的量化論斷均通過 Grep 核對，**無 ❌GREP_FAIL 項目**。僅有 2 項「待議」為表述精確度層級的建議，不影響論證正確性。
