# 真實臨床的 combination logic · FIDELITY / FINEARTS-HF / FLOW 的旁證

> **本檔定位**：本檔為主題三（第四支柱還是提早聯用？）主文 §3「真實臨床的 combination logic」之延伸拆解。主文該節僅以約 15% 篇幅帶過 FIDELITY / FINEARTS-HF / FLOW 的 subgroup 旁證；本檔把這些長期 outcome 試驗的次分析**逐一交代研究設計、效應量＋CI＋P、並區分 prespecified / post hoc / exploratory**，回答一個 CONFIDENCE（180 天、只測 UACR）無法回答的問題：**「聯用在 hard endpoint 上是否 additive，且各支柱的分工與安全性如何？」**
>
> **引用標記慣例**：📄 = 本地握有經查核之全文、可 grep 稽核；📌 = 僅有 abstract。對 📌 來源不作其未載內容之具體斷言。每一事實句末以 `[本地MD檔名]` 標註供 grep 回溯。LLM 僅負責組織與改寫，所有數字／HR／CI／P／n 均出自本地全文 MD。
>
> **證據分層**：🟢 guideline routine（已進指引常規）｜🟡 evidence expansion（prespecified subgroup／post hoc／surrogate／actuarial 模型）｜🔴 hypothesis（僅機轉合理、無隨機化 hard-outcome 佐證）。
>
> **與統計視角勿重複**：本檔聚焦「combination logic 的旁證證據」；各文獻的統計迷思（subgroup 交互作用的統計陷阱、surrogate 效度）見同資料夾 [`statistical_insights_myths.md`](statistical_insights_myths.md)，此處不重述。

---

## 0. 為什麼需要「旁證」——CONFIDENCE 的三個邊界

CONFIDENCE 是唯一針對「同步起始」隨機化的試驗，但它有三個結構性限制，使得「聯用邏輯」的臨床論證必須借助更長期試驗的次分析來補：

1. **只有 180 天**——無法觀察 hard renal / CV outcome。
2. **主終點是 UACR**——一個 surrogate。
3. **只比 finerenone × SGLT2i**——沒有回答 GLP-1RA 在四支柱裡補什麼。

FIDELITY（T2D+CKD，中位追蹤 3.0 年）、FINEARTS-HF（HFmrEF/HFpEF，中位追蹤 2.6 年）、FLOW（T2D+CKD 腎臟結局，中位追蹤 3.4 年）三個 outcome 試驗的 subgroup / post hoc 分析，正好補上這三個缺口——但**代價是它們都不是為「聯用」而隨機化、也不是為交互作用而 power**（見 §6 誠實邊界）。

---

## 1. FIDELITY × SGLT2i：finerenone 的心腎益處不因 SGLT2i 而異（Rossing 2022）🟡

### 1.1 研究設計

FIDELITY 是 FIDELIO-DKD（NCT02540993）與 FIGARO-DKD（NCT02545049）兩個隨機、雙盲、安慰劑對照 phase 3 試驗的**預先設定（prespecified）個體病人層級匯總分析**，共 **13,026 名** T2D+CKD、全部在最大耐受 RASi 背景下、篩選時血鉀 ≤4.8 mmol/L 者，1:1 隨機分入 finerenone（10/20 mg OD 滴定）或 matching placebo [sglt2i_subgroup_FIDELITY_Rossing_2022] 📄。本次 SGLT2i 分析中，**877 名（6.7%）於基線使用 SGLT2i**（finerenone 組 438、placebo 組 439），另 **1,113 名（8.5%）於試驗期間起始 SGLT2i**；SGLT2i 使用**未被隨機化、未作分層**，故為觀察性次組 [sglt2i_subgroup_FIDELITY_Rossing_2022] 📄。主要療效終點為 CV 複合（CV death、nonfatal MI、nonfatal stroke、HHF）與腎臟複合（kidney failure、持續 ≥57% eGFR 下降、renal death），由獨立且盲性的事件委員會裁定；分析於 pooled full analysis set 進行，並以 Cox 模型校正基線 HbA1c、SBP、log-UACR、eGFR [sglt2i_subgroup_FIDELITY_Rossing_2022] 📄。

### 1.2 效應量：方向一致，交互作用皆不顯著

**表 1｜FIDELITY 依基線 SGLT2i 使用之 finerenone vs placebo 效應（校正後 HR）**

| 終點 | 無 SGLT2i（n≈12,149）HR (95% CI) | 有 SGLT2i（n=877）HR (95% CI) | P-interaction |
|---|---|---|---|
| CV 複合 | 0.87 (0.79–0.96) | 0.67 (0.42–1.07) | 0.46 |
| 腎臟複合 | 0.80 (0.69–0.92) | 0.42 (0.16–1.08) | 0.29 |
| HHF（post hoc 單項） | 0.80 (0.68–0.95) | 0.44 (0.19–0.99) | 0.18 |
| All-cause death | 0.90 (0.80–1.02) | 0.58 (0.30–1.10) | 0.24 |

（全數 [sglt2i_subgroup_FIDELITY_Rossing_2022] 📄；有 SGLT2i 組點估計看似更低，但 CI 極寬、且四個 P-interaction 均不顯著，故只能解讀為「不因 SGLT2i 而異」，**不能**解讀為「加 SGLT2i 讓 finerenone 更有效」。）

**on-treatment（把 SGLT2i 當 time-varying covariate）分析**同向：CV 複合有使用 0.77（0.51–1.15）vs 無使用 0.82（0.73–0.91），Pinteraction 0.77；腎臟複合 0.92（0.41–2.08）vs 0.69（0.58–0.83），Pinteraction 0.50 [sglt2i_subgroup_FIDELITY_Rossing_2022] 📄。唯一達顯著交互作用者為 on-treatment 之 HHF（有使用 0.18〔0.06–0.53〕vs 無使用 0.71〔0.58–0.86〕，Pinteraction 0.015），惟事件數極少（有使用組僅 4 vs 23 事件），須謹慎 [sglt2i_subgroup_FIDELITY_Rossing_2022] 📄。

### 1.3 surrogate 與安全：UACR、eGFR、血鉀

- **UACR（baseline→month 4）**：有 SGLT2i 者 finerenone 較 placebo 降 **37%（ratio 0.63；95% CI 0.57–0.70）**、無 SGLT2i 者降 **31%（ratio 0.69；0.67–0.71）**，Pinteraction 0.17 [hyperkalemia_combo_Rossing_2022] 📄。
- **急性 eGFR（baseline→month 4 組間差）**：有 SGLT2i −3.69、無 SGLT2i −2.23、兩者差 −1.46 mL/min/1.73 m²（95% CI −1.89 到 −1.04）——即併用 SGLT2i 時初期 dip 略深，符合兩藥血流動力學可加 [hyperkalemia_combo_Rossing_2022] 📄。
- **慢性 eGFR slope（month 4→EOS）**：有 SGLT2i 者 finerenone −1.92（95% CI −2.61 到 −1.23）vs placebo −3.45（−4.15 到 −2.76）；無 SGLT2i 者 finerenone −2.54 vs placebo −3.72；finerenone vs placebo 的組間益處在**有 SGLT2i 者反而更大（1.54 vs 1.18 mL/min/1.73 m²）** [sglt2i_subgroup_FIDELITY_Rossing_2022] 📄。
- **高血鉀（慢性 SGLT2i 背景下較低）**：任何高血鉀 AE 在有 SGLT2i 者 finerenone **10.3%（45/438）vs placebo 2.7%（12/439）**、無 SGLT2i 者 **14.3%（867/6,072）vs 7.2%（436/6,050）**；中央實驗室 K >5.5 在有 SGLT2i 者 **7.9%（34）vs 3.0%（13）**、無 SGLT2i 者 **17.4%（1,041）vs 7.7%（457）** [sglt2i_subgroup_FIDELITY_Rossing_2022] 📄。**關鍵**：在有 SGLT2i 者，finerenone 與 placebo 的高血鉀致停藥率相近（1.1% vs 0.7%），且血清鉀組間無差異 [sglt2i_subgroup_FIDELITY_Rossing_2022] 📄。

> **旁證的重量與限度**：FIDELITY 是本檔唯一提供 finerenone **hard endpoint** 的來源，且方向一致（心、腎、HHF、死亡的點估計在有 SGLT2i 者皆 ≤ 無 SGLT2i 者）；但 SGLT2i 使用為**慢性、觀察性**背景，並非同步起始，故「較低高血鉀」不能外推到 CONFIDENCE 式的同步起始情境（見 §4 與主文 §2.4）。

---

## 2. FIDELITY × 三藥（SGLT2i＋GLP-1RA）：post hoc 的最深旁證（Singh 2026）🟡

### 2.1 設計與族群

Singh 為 FIDELITY 的 **post hoc** 次分析，把 **12,990 名**依基線併用藥分四組：合併 SGLT2i＋GLP-1RA **n=167（1.3%）**、SGLT2i-only **706（5.4%）**、GLP-1RA-only **776（6.0%）**、皆無 **11,341（87.3%）**；中位追蹤 **3.0 年（IQR 2.3–3.8）** [hyperkalemia_combo_Singh_2026] 📄。三藥組基線 UACR 較低（441.8 vs 皆無組 522.7 mg/g）、eGFR 較高（64.9 vs 56.9 mL/min/1.73 m²），反映其 CKD 期別較早——此即後述 confounding by indication 的來源 [hyperkalemia_combo_Singh_2026] 📄。

### 2.2 效應量（surrogate）

- **UACR month 4（finerenone vs placebo 降幅）**：三藥 **38%**、皆無 **31%**、SGLT2i-only **37%**、GLP-1RA-only **38%**；三藥組於 month 12 觀察到最大降幅 [hyperkalemia_combo_Singh_2026] 📄。
- **UACR month 24（LS-mean 治療比）**：三藥 **0.43（95% CI 0.31–0.59；P<0.0001）**、皆無 0.62（0.59–0.65）、SGLT2i-only 0.63（0.52–0.76）、GLP-1RA-only 0.61（0.51–0.71）——三藥組降幅最大 [hyperkalemia_combo_Singh_2026] 📄。
- **急性 eGFR month 1（LS-mean 治療差）**：三藥 **−4.22（95% CI −7.28 到 −1.15）**，深於皆無 −2.19（−2.48 到 −1.90）、SGLT2i-only −2.39、GLP-1RA-only −1.38——藥越多、初期 dip 越明顯 [hyperkalemia_combo_Singh_2026] 📄。
- **慢性 eGFR slope**：三藥 1.19 mL/min/1.73 m²/yr（95% CI −0.18 到 2.56，**P=0.089，不顯著**）、皆無 1.02（0.84–1.20，P<0.0001）、SGLT2i-only 0.88（0.07–1.69，P=0.034）、GLP-1RA-only 1.26（0.59–1.92，P=0.0002）——三藥組因 n 小而未達顯著 [hyperkalemia_combo_Singh_2026] 📄。
- **SBP month 4**：三藥降幅最大 **−5.77 mmHg（95% CI −10.06 到 −1.48，P=0.0085）**，皆無 −3.63、SGLT2i-only −2.69、GLP-1RA-only −3.76 [hyperkalemia_combo_Singh_2026] 📄。

### 2.3 安全（慢性 SGLT2i 背景再度降鉀）

investigator-reported 高血鉀在 finerenone > placebo 於各組皆然（整體 14.0% vs 6.9%）；但**含 SGLT2i 的組別事件率較低**：SGLT2i-only 9.4% vs 2.0%、三藥 14.0% vs 6.2%，對比皆無組 14.2% vs 7.1% [hyperkalemia_combo_Singh_2026] 📄。實驗室 K >5.5 亦然：SGLT2i-only **7.9% vs 2.8%**、三藥 **8.1% vs 3.8%**，遠低於皆無組 **17.7% vs 7.9%** [hyperkalemia_combo_Singh_2026] 📄。三藥組因 finerenone 致停藥／住院之高血鉀為 0 例 [hyperkalemia_combo_Singh_2026] 📄。

> **性質誠實**：Singh 為 **post hoc、exploratory**；作者自陳三藥組 n=167 過小、12 個月後樣本不足以做正式組間比較，結論為 **hypothesis-generating**，須大型 RCT 前瞻驗證 [hyperkalemia_combo_Singh_2026] 📄。三藥組「降鉀」同樣受慢性使用與 confounding by indication 影響（見 §6）。

---

## 3. FINEARTS-HF × SGLT2i：把旁證延伸到 HFmrEF/HFpEF（Vaduganathan 2025）🟡

### 3.1 設計

FINEARTS-HF（NCT04435626）是隨機、雙盲、安慰劑對照試驗，納入 **6,001 名** LVEF ≥40% 的 HFmrEF/HFpEF、eGFR ≥25、血鉀 ≤5.0 者，1:1 隨機分入 finerenone（依 baseline eGFR 給 20 或 40 mg OD）或 placebo；試驗中禁用其他 MRA [hyperkalemia_combo_Vaduganathan_2025] 📄。**基線 SGLT2i 使用是 prespecified subgroup**：817 名（13.6%）——這是 MRA 試驗中**跨疾病別納入 SGLT2i 使用者最多**的一次；中位追蹤 2.6 年 [hyperkalemia_combo_Vaduganathan_2025] 📄。主終點為 total（首發＋復發）worsening HF events 與 CV death 的複合 [hyperkalemia_combo_Vaduganathan_2025] 📄。

### 3.2 效應量與安全

- **主終點**：SGLT2i 使用者 RR **0.83（95% CI 0.60–1.16）**、非使用者 RR **0.85（0.74–0.98）**，Pinteraction **0.76**；因基線風險較高，SGLT2i 使用者**絕對事件減少反而近乎加倍（4.7 vs 2.5 事件/100 py）** [hyperkalemia_combo_Vaduganathan_2025] 📄。
- **血鉀**：1 個月時 finerenone 使血鉀上升 **+0.19 mmol/L**，有 SGLT2i（0.13–0.25）與無 SGLT2i（0.17–0.21）**完全相同（Pinteraction 1.00）**；實驗室 K >5.5 在無 SGLT2i 者 fin 14.2% vs pbo 7.1%、有 SGLT2i 者 fin 14.5% vs pbo 5.6% [hyperkalemia_combo_Vaduganathan_2025] 📄。此與 CONFIDENCE「同步起始不抵消血鉀」方向一致（見主文 §2.4）。
- **SGLT2i drop-in 不對稱**：試驗中 980 名（18.9%）起始 SGLT2i，finerenone 組較 placebo 組少（**17.7% vs 20.1%；HR 0.86，95% CI 0.76–0.97；P=0.02**）——推測反映 placebo 組較常惡化而加藥；time-varying 校正後 finerenone 主終點療效不變（HR 0.85，0.76–0.95，P=0.003）[hyperkalemia_combo_Vaduganathan_2025] 📄。

### 3.3 一個必須誠實的「反例」：HFmrEF/HFpEF 沒有腎臟保護訊號

與 T2D+CKD 不同，**finerenone 在 FINEARTS-HF 未顯示腎臟複合終點益處**：無 SGLT2i 者 renal composite HR **1.43（95% CI 0.98–2.08）**、有 SGLT2i 者 **0.95（0.37–2.45）**，Pinteraction 0.37 [hyperkalemia_combo_Vaduganathan_2025] 📄。作者歸因於事件率低、追蹤較短、且 HF 與 DKD 的腎病進展機轉可能不同 [hyperkalemia_combo_Vaduganathan_2025] 📄。**這提醒：finerenone 的「腎保護」旁證主要來自 T2D+CKD 族群（FIDELITY），不可無條件外推到心衰族群的腎終點。**

---

## 4. GLP-1RA 補什麼：FLOW 的兩個 subgroup（Mann 2024 / Rossing 2025）🟡

FLOW（NCT03819153）是隨機、雙盲、安慰劑對照的**專用腎臟結局試驗**，**3,533 名** T2D+CKD 者 1:1 隨機分入 semaglutide 1.0 mg SC QW 或 placebo，主終點為五成分腎臟複合（持續 ≥50% eGFR 下降、kidney failure、腎或 CV 死亡）；整體 semaglutide 降腎臟複合 **24%（HR 0.76，95% CI 0.66–0.88）**、MACE 降 18%、all-cause death 降 20%、eGFR slope 減緩 1.16 mL/min/1.73 m²/yr [glp1_cardiorenal_Mann_2024] 📄 [glp1_cardiorenal_Rossing_2025] 📄。

### 4.1 FLOW × SGLT2i（Mann 2024，prespecified）

基線 SGLT2i 使用 **550 名（15.6%）**、無使用 2,983 名 [glp1_cardiorenal_Mann_2024] 📄。主終點：有 SGLT2i **41/277 vs 38/273，HR 1.07（95% CI 0.69–1.67；P=0.755）**、無 SGLT2i **HR 0.73（0.63–0.85；P<0.001）**，**Pinteraction 0.109** [glp1_cardiorenal_Mann_2024] 📄。MACE、all-cause death 的 Pinteraction 分別 0.741、0.901，eGFR slope Pinteraction 0.237——semaglutide 益處不因 SGLT2i 而異 [glp1_cardiorenal_Mann_2024] 📄。

> **判讀重點**：SGLT2i 亞組點估計 1.07 看似「無效」，但**該組僅 550 人、事件少（41 vs 38）、CI 極寬跨越 1**，且 Pinteraction 0.109 不顯著；正確結論是「無異質性」，不是「semaglutide 對 SGLT2i 使用者無效」——此為典型 subgroup 統計陷阱（詳見 [`statistical_insights_myths.md`](statistical_insights_myths.md)）。

### 4.2 FLOW × MRA（Rossing 2025，prespecified）— 一個重要的字面陷阱

基線 MRA 使用 **257 名（7.3%）**、無使用 3,276 名。**關鍵誠實**：這裡的 MRA **絕大多數是類固醇型 MRA**（spironolactone 218 名〔84.8%〕、eplerenone 38 名〔14.8%〕、esaxerenone 1 名），**finerenone 為 0 名**（finerenone 2021 年 7 月才核准、FLOW 招募已結束）[glp1_cardiorenal_Rossing_2025] 📄。主終點：MRA 使用者 **HR 0.51（95% CI 0.30–0.86；23/136 vs 36/121）**、非使用者 **HR 0.79（0.68–0.92）**，Pinteraction **0.12**；MACE 與 all-cause death 的 Pinteraction 均 >0.7 [glp1_cardiorenal_Rossing_2025] 📄。血鉀（>5.5）在 semaglutide vs placebo 無交互作用（MRA 使用者 22.1% vs 19.0%、非使用者 13.6% vs 17.6%；Pinteraction 0.12）[glp1_cardiorenal_Rossing_2025] 📄。

> **邊界**：主文以「基線 MRA 有 HR 0.51 vs 無 0.79」佐證 GLP-1RA 與 MRA 可加，方向正確；但必須標明此 MRA **並非 finerenone**，故只能說「GLP-1RA 益處不因（類固醇型）MRA 背景而異」，對「semaglutide + finerenone」僅為**間接類推**。FIDELITY 中 finerenone 益處在 944 名 GLP-1RA 使用者與 12,082 名非使用者間無顯著交互作用，是另一半的旁證 [glp1_cardiorenal_Rossing_2025] 📄。

### 4.3 GLP-1RA 的分工

FLOW 證實 GLP-1RA 也參與腎保護（本業之外），且益處不因 SGLT2i / MRA 背景而異——支持其作為第四支柱**疊加**而非取代 SGLT2i/finerenone 的腎/HHF 角色 [glp1_cardiorenal_Mann_2024] 📄 [glp1_cardiorenal_Rossing_2025] 📄。這與 Neuen 的事件型態分工（GLP-1RA 主補 ASCVD、對 HHF 較弱；見主文表 3 與 §5）互補。

---

## 5. 把四支柱疊起來會怎樣：Neuen 的 lifetime actuarial 模型（Neuen 2024）🟡

Neuen 以 **actuarial（age-based）跨試驗間接比較**，把三類藥的效應疊在 CANVAS+CREDENCE 的 placebo 族群上模擬。資料來源：2 個 SGLT2i 試驗（CANVAS+CREDENCE，n=14,543）、8 個 GLP-1RA 試驗的 trial-level meta（n=60,080）、2 個 nsMRA 試驗（FIDELIO+FIGARO，n=13,026）；absolute 估計基於 3,482 名 UACR ≥30 mg/g、接受 conventional care 者 [glp1_cardiorenal_Neuen_2024] 📄。

**表 2｜三藥合用 vs conventional care 之估計 HR（完全可加假設）**

| 終點 | SGLT2i 單獨 | GLP-1RA 單獨 | nsMRA 單獨 | 三藥合用 HR (95% CI) |
|---|---|---|---|---|
| MACE | 0.83 | 0.86 | 0.90 | **0.65 (0.55–0.76)** |
| HHF | 0.64 | 0.89 | 0.78 | **0.45 (0.34–0.58)** |
| CKD 進展 | 0.63 | 0.86 | 0.77 | **0.42 (0.31–0.56)** |
| CV death | 0.84 | 0.87 | 0.88 | **0.64 (0.51–0.80)** |
| All-cause death | 0.85 | 0.88 | 0.89 | **0.67 (0.55–0.80)** |

（全數 [glp1_cardiorenal_Neuen_2024] 📄。此表也量化了分工：HHF 由 SGLT2i〔0.64〕主導、nsMRA〔0.78〕次之、GLP-1RA〔0.89〕最弱。）

**絕對益處（3 年）**：MACE 的 ARR **4.4%（95% CI 3.0–5.7）**、NNT **23（18–33）** [glp1_cardiorenal_Neuen_2024] 📄。**壽命增益（50 歲起始三藥 vs conventional care）**：MACE-free survival **+3.2 年（2.1–4.3）**、HHF-free **+3.2 年（2.4–4.0）**、CKD 進展-free **+5.5 年（4.0–6.7）**、CV survival **+2.2 年（1.2–3.0）**、overall survival **+2.4 年（1.4–3.4）** [glp1_cardiorenal_Neuen_2024] 📄。即使**保守假設只有 50% additivity**，MACE 仍 +2.4 年（1.1–3.5）、CKD 進展 +4.5 年（2.8–5.9）、all-cause death +1.8 年（0.7–2.8）[glp1_cardiorenal_Neuen_2024] 📄。益處隨起始年齡遞減（55/60/65 歲之 MACE 增益 2.7 / 2.1 / 1.3 年）[glp1_cardiorenal_Neuen_2024] 📄。

> **性質誠實（最重要）**：Neuen 為 **cross-trial 間接比較 + actuarial 外推模型**，其核心假設為「各藥效應獨立且可加（log-HR 相加）」；作者自陳若機轉重疊則可能 sub-additive，故並列 50% additivity 敏感度分析 [glp1_cardiorenal_Neuen_2024] 📄。**這不是任何 head-to-head RCT 的結果**，屬 🟡→🔴 之間的 evidence expansion，僅供 shared decision making 參考，不可當成三藥聯用之硬終點證明。

---

## 6. 誠實邊界（Evidence limits）🟡🔴

1. **全部是非隨機化的併用**。FIDELITY、FINEARTS-HF、FLOW 均**只隨機化 finerenone/semaglutide vs placebo**，SGLT2i / GLP-1RA / MRA 使用皆為**觀察性次組、未分層、未為交互作用而 power**；CONFIDENCE 的隨機化才是唯一無此偏誤者 [sglt2i_subgroup_FIDELITY_Rossing_2022] 📄 [hyperkalemia_combo_Vaduganathan_2025] 📄。
2. **Confounding by indication 可量化**。FIDELITY 中基線用 SGLT2i 者 eGFR 較高（66.3±21.1 vs 57.0±21.6）、UACR 較低（中位 448 vs 521 mg/g）、GLP-1RA 使用率約三倍（19.0% vs 6.4%）——這正是 with-SGLT2i 亞組安慰劑事件率偏低、須以 P-interaction 而非組間點估計解讀的原因 [sglt2i_subgroup_FIDELITY_Rossing_2022] 📄。Singh 的三藥組同樣 CKD 期別較早 [hyperkalemia_combo_Singh_2026] 📄。
3. **「較低高血鉀」屬慢性背景，不能外推同步起始**。FIDELITY / Singh / FINEARTS-HF 觀察到的 SGLT2i 降鉀，是**慢性（已在用）SGLT2i** 的現象；CONFIDENCE 的隨機化同步起始並未複製此降鉀。Sinclair 的時序假說（FIVE-STAR：已用 SGLT2i 者再加 finerenone 血鉀僅升 0.13 vs 未用者 0.37 mEq/L；Pinteraction 0.02）提供機轉調和，但**仍屬 hypothesis-generating**，FIVE-STAR 之 SGLT2i 使用非隨機 [hyperkalemia_combo_Sinclair_2026] 📄。
4. **FLOW 的 MRA 是類固醇型、非 finerenone** 🔴。FLOW × MRA 的 0.51 vs 0.79 只能支持「GLP-1RA + 類固醇型 MRA」，對 finerenone 為間接類推 [glp1_cardiorenal_Rossing_2025] 📄。
5. **surrogate 邊界** 🟡。UACR / eGFR slope / SBP 為代理終點；FIDELITY 提供的 hard endpoint 亦為次組、CI 寬。
6. **Neuen 為模型外推** 🔴。假設效應可加、class effect 成立、long-term 外推——非任何實測聯用試驗。
7. **finerenone 腎保護不可跨疾病外推**：FINEARTS-HF（HFmrEF/HFpEF）未見腎臟複合益處（HR 1.43 / 0.95，Pint 0.37），提醒 T2D+CKD 的腎旁證有其族群邊界 [hyperkalemia_combo_Vaduganathan_2025] 📄。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|------|------|------------------|
| finerenone 心腎益處不因（慢性）SGLT2i 而異（CV 0.87/0.67、腎 0.80/0.42，Pint 0.46/0.29） | 🟡 prespecified subgroup | `sglt2i_subgroup_FIDELITY_Rossing_2022` 📄 |
| 慢性 SGLT2i 背景下 finerenone 高血鉀較低（K>5.5：7.9% vs 17.4%） | 🟡 觀察性次組 | `sglt2i_subgroup_FIDELITY_Rossing_2022` / `hyperkalemia_combo_Rossing_2022` 📄 |
| 三藥背景 UACR 降幅最大（month 24 ratio 0.43） | 🟡 post hoc | `hyperkalemia_combo_Singh_2026` 📄 |
| HFmrEF/HFpEF 中 finerenone 益處不因 SGLT2i 而異（RR 0.83/0.85，Pint 0.76） | 🟡 prespecified subgroup | `hyperkalemia_combo_Vaduganathan_2025` 📄 |
| 同步/慢性血鉀：1 個月 +0.19 mmol/L 有無 SGLT2i 相同（Pint 1.00） | 🟡 | `hyperkalemia_combo_Vaduganathan_2025` 📄 |
| finerenone 在心衰族群無腎臟複合益處（HR 1.43/0.95） | 🟡（誠實反例） | `hyperkalemia_combo_Vaduganathan_2025` 📄 |
| GLP-1RA 益處不因 SGLT2i 而異（腎 0.73/1.07，Pint 0.109） | 🟡 prespecified subgroup | `glp1_cardiorenal_Mann_2024` 📄 |
| GLP-1RA 益處不因（類固醇型）MRA 而異（腎 0.79/0.51，Pint 0.12） | 🟡 prespecified subgroup | `glp1_cardiorenal_Rossing_2025` 📄 |
| 三藥 lifetime 益處（CKD 進展 +5.5 年、MACE HR 0.65） | 🔴 actuarial 模型外推 | `glp1_cardiorenal_Neuen_2024` 📄 |
| SGLT2i 先行以降鉀（時序假說） | 🔴 hypothesis | `hyperkalemia_combo_Sinclair_2026` 📄 |
| 同步三藥聯用之 hard-outcome RCT | 🔴 尚無 | —（誠實揭露；PRECIDENTD / CONFIRMATION-HF 進行中） |

## 本地全文語料（可 grep 稽核）

📄 全文：`sglt2i_subgroup_FIDELITY_Rossing_2022`（FIDELITY × SGLT2i 完整表格版）、`hyperkalemia_combo_Rossing_2022`（同篇之數字摘錄版）、`hyperkalemia_combo_Singh_2026`（FIDELITY × SGLT2i+GLP-1RA 三藥 post hoc）、`hyperkalemia_combo_Vaduganathan_2025`（FINEARTS-HF × SGLT2i prespecified）、`hyperkalemia_combo_Sinclair_2026`（時序假說 editorial）、`glp1_cardiorenal_Mann_2024`（FLOW × SGLT2i prespecified）、`glp1_cardiorenal_Rossing_2025`（FLOW × MRA prespecified）、`glp1_cardiorenal_Neuen_2024`（lifetime actuarial 模型）。交叉連結：`statistical_insights_myths.md`（subgroup 統計陷阱、surrogate 效度）。

---

## References（Vancouver + 本地檔名）

1. Rossing P, Anker SD, Filippatos G, et al. Finerenone in patients with chronic kidney disease and type 2 diabetes by sodium–glucose cotransporter 2 inhibitor treatment: the FIDELITY analysis. Diabetes Care. 2022;45(12):2991–2998. doi:10.2337/dc22-0294. 📄 [sglt2i_subgroup_FIDELITY_Rossing_2022] / [hyperkalemia_combo_Rossing_2022]
2. Singh AK, Anker SD, Pitt B, et al. A FIDELITY analysis on finerenone with SGLT-2i and GLP-1RA in CKD. Kidney Int Rep. 2026. doi:10.1016/j.ekir.2025.10.032. 📄 [hyperkalemia_combo_Singh_2026]
3. Vaduganathan M, Claggett BL, Kulac IJ, et al. Effects of the nonsteroidal MRA finerenone with and without concomitant SGLT2 inhibitor use in heart failure (FINEARTS-HF). Circulation. 2025;151(2):149–158. doi:10.1161/CIRCULATIONAHA.124.072055. 📄 [hyperkalemia_combo_Vaduganathan_2025]
4. Mann JFE, Rossing P, Bakris G, et al. Effects of semaglutide with and without concomitant SGLT2 inhibitor use in participants with type 2 diabetes and chronic kidney disease in the FLOW trial. Nat Med. 2024;30(10):2849–2856. doi:10.1038/s41591-024-03133-0. 📄 [glp1_cardiorenal_Mann_2024]
5. Rossing P, Bakris G, Perkovic V, et al. Effects of semaglutide with or without concomitant mineralocorticoid receptor antagonist use in participants with type 2 diabetes and chronic kidney disease: a FLOW trial prespecified secondary analysis. Diabetes Care. 2025. doi:10.2337/dc25-0472. 📄 [glp1_cardiorenal_Rossing_2025]
6. Neuen BL, Heerspink HJL, Vart P, et al. Estimated lifetime cardiovascular, kidney, and mortality benefits of combination treatment with SGLT2 inhibitors, GLP-1 receptor agonists, and nonsteroidal MRA compared with conventional care in patients with type 2 diabetes and albuminuria. Circulation. 2024;149(6):450–462. doi:10.1161/CIRCULATIONAHA.123.067584. 📄 [glp1_cardiorenal_Neuen_2024]
7. Sinclair MR, Edmonston D. It's about time: potassium risk with combination guideline-directed medical therapy. Kidney Int Rep. 2026;11:106609. doi:10.1016/j.ekir.2026.106609. 📄 [hyperkalemia_combo_Sinclair_2026]

---

*此檔為主題三主文 §3 之延伸拆解，撰寫基準日 2026-07-12。所有具體數字均可 grep 回上列本地全文 MD。本節旁證多為 prespecified subgroup / post hoc / actuarial 模型、以觀察性併用與 surrogate 為主；「同步三藥聯用」之 hard-outcome 隨機化證據目前不存在（PRECIDENTD、CONFIRMATION-HF 進行中），屬明示之研究缺口。*
