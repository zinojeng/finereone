# Claim Audit — 06_beyond_t2d_cardiorenal_landscape.md

**稽核員**: claim-auditor (Phase B, 三位並行稽核員之一)
**方法**: 逐句抽取百分比、樣本數、HR/OR/RR/CI、引號字串,對句尾 `[本地MD檔名]` 標記之來源檔於 `原始PDF/` 執行 grep 比對。
**結論**: 全文逐條核對後,**未發現 GREP_FAIL 項目**。所有可稽核的數字型陳述(樣本數、百分比、HR/RR/OR、95% CI、P 值)均可於對應本地 MD 檔案中逐字或語意等價命中;未發現研究設計誤植(如 cohort 誤標為 RCT)或引號捏造。

---

## 逐段稽核紀錄

### 第 1 節:T2D-CKD 背景
| 陳述 | 來源檔 | Grep 結果 |
|---|---|---|
| FIDELIO-DKD n=5734 | FIDELIO-DKD_NEJMoa2025845.md | ✅ 命中(line 17, 112) |
| 腎複合 HR 0.82 (0.73–0.93, P=0.001) | 同上 | ✅ 命中(line 21, 122, 390, 606-607) |
| CV 次要 HR 0.86 (0.75–0.99, P=0.03) | 同上 | ✅ 命中(line 21, 124, 660) |
| FIGARO-DKD n=7437 | FIGARO-DKD_NEJMoa2110956.md | ✅ 命中(line 33, 115) |
| CV 複合 HR 0.87 (0.76–0.98, P=0.03) | 同上 | ✅ 命中(line 33, 123, 454, 790) |
| HHF HR 0.71 (0.56–0.90) | 同上 | ✅ 命中(line 33, 123, 731, 826) |
| FIDELITY N=13,026(排除 GCP violation) | FIDELITY_Agarwal_2022.md | ✅ 命中(line 27:"N = 13,026") |
| CV HR 0.86 (0.78–0.95, P=0.0018) | 同上 | ✅ 命中(line 46) |
| 腎 HR 0.77 (0.67–0.88, P=0.0002) | 同上 | ✅ 命中(line 51) |
| ESKD 降 20%,HR 0.80 (0.64–0.99) | 同上 | ✅ 命中(line 57, 82) |
| KDIGO 2A 級建議,疊加最大耐受 RASi(±SGLT2i) | fine_heart_pooled_Vaduganathan_2024.md | ✅ 命中(line 49:"class 2A recommendation"…"maximally tolerated renin–angiotensin system inhibitors and/or SGLT2 inhibitors") |
| AHA 2023 Presidential Advisory,四階段連續光譜 | finearts_hfpef_ckm_Claudel_2023.md | ✅ 命中(line 22, 38:"four-stage grading system…ultimately converges on clinical CVD") |

### 第 2 節:FINE-ONE(T1D-CKD)
| 陳述 | 來源檔 | Grep 結果 |
|---|---|---|
| 20–30% 美國 T1D 成人合併 CKD | fine_one_t1d_Bayer_2026.md | ✅ 命中(line 34, 80) |
| FINE-ONE n=242,eGFR 25–<90,UACR 200–<5000,已用 ACEi/ARB | fine_one_t1d_Heerspink_2026.md | ✅ 命中(line 23, 25, 33, 35) |
| primary 6 個月 UACR 相對變化 | 同上 | ✅ 命中(line 23) |
| finerenone UACR −34%(GMR 0.66, 0.60–0.73);placebo −12%(GMR 0.88, 0.79–0.98) | 同上 | ✅ 命中(line 25) |
| placebo-corrected ~25%(GMR 0.75, 0.65–0.87, P<0.001) | 同上 | ✅ 命中(line 25) |
| 高血鉀 10.1% vs 3.3%;1.7% 因高血鉀停藥 vs 0% | fine_one_t1d_Heerspink_2026.md + fine_one_t1d_Bayer_2026.md | ✅ 命中(Heerspink line 27; Bayer line 58, 89-90:"1.7% vs 0%") |
| 6 個月 eGFR 變化 −5.6 vs −2.7(差 −2.9, −5.1至−0.7) | fine_one_t1d_Heerspink_2026.md | ✅ 命中(line 27, 40) |
| Beernink:UACR 效果不因 HbA1c 三分位(P int 0.41)或病程(P int 0.70)而異 | fine_one_t1d_Beernink_2026.md | ✅ 命中(line 33) |
| 6 個月 HbA1c 未變(+0.04%, P=0.74) | 同上 | ✅ 命中(line 33) |
| UACR 為 bridging biomarker,經法規回饋同意採用 | fine_one_t1d_Heerspink_2023.md | ✅ 命中(line 28) |
| FDA 2026-05 接受 sNDA、授予 Priority Review;若獲准為首個 T1D-CKD MRA | fine_one_t1d_Bayer_2026.md | ✅ 命中(line 28, 76:"would be the first nonsteroidal mineralocorticoid receptor antagonist") |

### 第 3 節:FIND-CKD(非糖尿病 CKD)
| 陳述 | 來源檔 | Grep 結果 |
|---|---|---|
| n=1584(793/791),eGFR 25–<90,UACR 200–≤3500,已用 RASi | find_ckd_nondiab_Heerspink_2026.md | ✅ 命中(line 24, 27, 36) |
| primary total eGFR slope 至 month 32 | 同上 | ✅ 命中(line 24) |
| 慢性腎絲球腎炎 57.0%(IgAN 26.3%),高血壓/缺血性腎病 29.0%,約半數腎切片確診 | glomerular_subgroup_Heerspink_2025.md | ✅ 命中(line 23, 95-97, 104:49.7%≈半數) |
| slope −3.3(−3.6至−3.1) vs −4.0(−4.3至−3.8),差 0.7(0.3–1.1, P<0.001) | find_ckd_nondiab_Heerspink_2026.md | ✅ 命中(line 27, 38) |
| 階層次要 cardiorenal HR 0.77(0.60–0.99, P=0.04) | 同上 | ✅ 命中(line 27) |
| 腎臟複合 HR 0.78(0.60–1.01);CV 複合 HR 0.60(0.27–1.33) | 同上 | ✅ 命中(line 27) |
| 高血鉀 17.0% vs 13.3%;停藥 1.5% vs 0.1%;住院 0.9% vs 0.6% | 同上 | ✅ 命中(line 27) |
| 66 RCT meta-analysis;0.75 mL/min/1.73m²/年對應 57% 下降中位 HR 0.74 | glomerular_subgroup_Heerspink_2025.md | ✅ 命中(line 158) |

### 第 4 節:Glomerular disease 亞群
| 陳述 | 來源檔 | Grep 結果 |
|---|---|---|
| 903 名(57.0%)glomerular disease;IgAN 416(46.1%)、FSGS 215(23.8%)、MN 90(10.0%);finerenone 446 vs placebo 457 | glomerular_subgroup_Neuen_2026.md | ✅ 命中(line 30, 36, 46-50) |
| slope −3.50 vs −4.23(差 0.73, 0.22–1.24) | 同上 | ✅ 命中(line 36) |
| month 12 白蛋白尿 −42%(35%–48%) | 同上 | ✅ 命中(line 36) |
| kidney failure/≥40% eGFR 下降 7.42 vs 9.60/100 py,HR 0.74(0.57–0.97) | 同上 | ✅ 命中(line 36) |

### 第 5 節:HFpEF/HFmrEF 與 CKM pooling
| 陳述 | 來源檔 | Grep 結果 |
|---|---|---|
| LVEF 光譜一致:<50% RR 0.84、50–<60% RR 0.80、≥60% RR 0.94;P int(類別)0.70;連續 P int 0.28 | finearts_hfpef_ckm_Docherty_2025.md | ✅ 命中(line 26,104-107) |
| n=6001(FINEARTS-HF) | finearts_baseline_ejhf_Solomon_2024.md / hf_finearts_Docherty_2025.md | ✅ 命中(多處) |
| HF 族群腎複合未降:75 vs 55 事件,HR 1.33(0.94–1.89) | finearts_hfpef_ckm_Mc_2025.md | ✅ 命中(line 443, 729-730) |
| acute eGFR dip −2.9;chronic slope +0.2(−0.1至+0.4);total slope 差 −0.7 | 同上 | ✅ 命中(line 446-448, 769-777) |
| 新發微量/巨量白蛋白尿降 24%/38% | 同上 | ✅ 命中(line 454:HR 0.76=24%降;HR 0.62=38%降) |
| FINE-HEART N=18,991,中位追蹤 2.9 年 | fine_heart_pooled_Vaduganathan_2024.md | ✅ 命中(line 20, 34, 36) |
| Primary CV 死亡 HR 0.89(0.78–1.01, P=0.076);敏感度 HR 0.88(0.79–0.98, P=0.025) | 同上 | ✅ 命中(line 20, 36) |
| 全因死亡 HR 0.91(0.84–0.99, P=0.027);HHF HR 0.83(0.75–0.92, P<0.001);腎複合 HR 0.80(0.72–0.90, P<0.001);CV死亡或HHF HR 0.85(0.78–0.93) | 同上 | ✅ 命中(line 20, 36, 38) |
| P interaction=0.94(CKM 條件數);2307人(12.1%)三條件並存 | 同上 | ✅ 命中(line 34, 40) |
| 高血鉀永久停藥 1.3% vs 0.5%,住院 0.8% vs 0.2%,無高血鉀死亡;SAE 34.6% vs 36.6%,無 AKI 過量 | 同上 | ✅ 命中(line 42) |
| 新發 AF/AFL 286(3.9%) vs 345(4.7%),HR 0.83(0.71–0.97, P=0.019) | finearts_hfpef_ckm_Pabon_2025.md | ✅ 命中(line 64-65, 359, 485) |
| 猝死 418(2.2%),HR 0.81(0.67–0.98, P=0.034);伴隨 Ameri 2026 JACC editorial(doi 10.1016/j.jacc.2026.05.031) | finearts_hfpef_ckm_Foa_2026.md | ✅ 命中(line 32, 39-40) |
| JASN 子集 14,180 人;CV死亡或HHF HR 0.83(0.75–0.93, P=0.001);腎複合隨 UACR 升高而增大(P int=0.04);非糖尿病敏感度分析 HbA1c P int=0.59 | finearts_hfpef_ckm_Ostrominski_2026.md | ✅ 命中(line 41) |
| INFINITY 14,574 人;腎複合 HR 0.76(0.68–0.86);kidney failure 0.85(0.74–0.99);CV複合 0.80(0.70–0.91);HHF 0.78(0.66–0.92);CV死亡 0.82(0.67–0.999);全因死亡 0.88(0.79–0.99) | find_ckd_nondiab_Neuen_2026.md | ✅ 命中(line 27) |
| 引號「foundational therapy」 | 同上 | ✅ 命中(line 30:"…support finerenone as a foundational therapy for CKD…") |

### 表 6 / 森林圖 3 / References
- 表 6 與森林圖 3 中所有 HR/CI/樣本數皆為前述已驗證數字之重複引用,無新增數字,交叉核對一致(0.77/0.74/0.76/0.60/0.86/0.80/0.91/0.88 等均與各自來源檔逐一命中)。
- References 1–19 之 DOI 逐一與各本地 MD 檔案 frontmatter/內文之 doi 欄位比對,**全數命中**(FIDELIO/FIGARO/FIDELITY/FINE-ONE/Beernink/design paper/FIND-CKD/design NDT/glomerular JAMA/INFINITY Lancet/FINE-HEART/Docherty/Mc Causland/Pabon/Foà/Ostrominski JASN/Ostrominski JACC anthropometric/Claudel)。
- 核准日期:T2D-CKD「2021 起」與 HFpEF/HFmrEF「2025/07」均於 fine_one_t1d_Bayer_2026.md 命中("Since 2021"…, "July 2025: FDA approval…LVEF ≥40%")。
- FDA Priority Review 受理日期 2026-05 於 Bayer press release(May 21, 2026)與 Pharmacy Times(May 25, 2026)命中。

### 研究設計特別檢查
- FINE-ONE、FIND-CKD 皆於來源檔明確標示為 "phase 3" 隨機雙盲對照試驗(RCT),非 cohort 誤植——命中 fine_one_t1d_Heerspink_2026.md line 33("Phase 3 RCT")、find_ckd_nondiab_Heerspink_2026.md(randomized, double-blind)。
- FINE-HEART、INFINITY 明確標示為 pooled/IPD meta-analysis,主文亦以「pooled」「individual participant data meta-analysis」正確描述,未誤植為 RCT。
- Glomerular disease 亞群明確標示為 FIND-CKD 內之 prespecified exploratory subgroup,主文正確標註「exploratory」而非誇大為 confirmatory trial。

### 數字位數檢查
- 逐一核對樣本數之全部位數(5734/7437/13,026/242/1584/793/791/903/446/457/416/215/90/6001/18,991/14,180/14,574/2307)均與來源檔逐字相符,未發現位數偏移(如 n 誤植多一位數)之情形。

---

## 結論
本文所有可稽核之百分比、樣本數、HR/OR/RR/CI 與引號字串,經逐一 grep 比對 `原始PDF/` 對應本地 MD 檔案,**全數命中,無 ❌GREP_FAIL 項目**。研究設計標註(RCT vs pooled vs exploratory subgroup)與原文一致,未見誤植。DOI 與核准日期等後設資料亦交叉核對無誤。

**建議**:待其他兩位並行稽核員(如有針對方法學詮釋、引用完整性等不同角度)之發現後,由 arbitrator 彙整。就純粹「數字/引號可否 grep 回溯」此一稽核目標而言,本文品質達標,無需修正。
