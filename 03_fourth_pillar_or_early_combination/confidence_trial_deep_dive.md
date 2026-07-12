# CONFIDENCE 深度解析 · 第一個直接檢驗「同步起始」的三臂試驗

> 本檔為主題三（第四支柱還是提早聯用？）主文 §2 的**延伸拆解與學術完整版**：把 CONFIDENCE 從「一段核心資料」放大成一份可獨立閱讀的試驗解剖——研究設計、終點階層、效應量與信賴區間、機轉中介分析、血鉀反直覺結果，以及 surrogate 到 hard outcome 的證據邊界。統計迷思與轉換視角另見 [`statistical_insights_myths.md`](statistical_insights_myths.md)；急性 eGFR dip 的跨 class 對讀見 [`../05_hyperkalemia_egfr_dip_safety_engineering/egfr_dip_hemodynamic_reversible.md`](../05_hyperkalemia_egfr_dip_safety_engineering/egfr_dip_hemodynamic_reversible.md)。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（不對其未載內容作具體斷言）。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織與改寫，所有作者／年份／數字均出自本地 MD 檔。
>
> **證據分層**：🟢 guideline routine（已進指引常規）｜🟡 evidence expansion（surrogate／prespecified 次分析／post hoc／模型分析）｜🔴 hypothesis（機轉合理、尚無隨機化硬終點驗證）。
>
> **一句話定位**：CONFIDENCE 是**第一個以隨機化直接檢驗「finerenone + SGLT2i 同步起始」**的試驗。它在 albuminuria（surrogate）上給了乾淨、over-additive 的答案（🟡），卻同時戳破一個流行假說——同步加 SGLT2i 並不能抵消 finerenone 的高血鉀（🟡，反直覺）；而所有 hard renal/CV outcome 的優劣，它**沒有、也無力回答**（🔴）。

---

## 1. 研究設計的解剖：為什麼這個試驗「乾淨」

### 1.1 三臂、double-dummy、Phase 2 的用意 🟡

CONFIDENCE（NCT05254002）是**隨機、雙盲、double-dummy、國際多中心、三臂平行組、Phase 2**試驗，療程 **7.5–8.5 個月**（每位受試者）[confidence_trial_Green_2023] 📄。三臂以 **1:1:1** 分配：(i) finerenone（10 或 20 mg qd）+ empagliflozin 10 mg；(ii) finerenone（10 或 20 mg qd）+ empagliflozin-matching placebo；(iii) empagliflozin 10 mg + finerenone-matching placebo [confidence_trial_Green_2023] 📄。**double-dummy 是關鍵**：它讓「單藥」臂也吞下對應的安慰劑，使投藥者、病人、結果評估者對分組全盲，是本試驗能對「同步起始」做出無偏比較的設計核心 [confidence_trial_Agarwal_2025] 📄。

Finerenone 的起始劑量依 baseline eGFR：eGFR ≥60 起始 20 mg、<60 起始 10 mg；第 30 天後若血鉀 ≤4.8 mmol/L 且 eGFR 下降 <30% 允許上調至 20 mg [confidence_trial_Green_2023] 📄。隨機化依 **eGFR（<60 vs ≥60）與 UACR（≤850 vs >850 mg/g）** 分層，採互動式網路系統 [confidence_trial_Agarwal_2025] 📄。試驗設有 7 次預定訪視，UACR 由連續晨尿測量、血鉀與 eGFR 於中央實驗室分析，訪視排程為 Day 14、30、90、180，並於停藥後 30 天（Day 210）再測一次以評估可逆性 [confidence_trial_Green_2023][confidence_trial_Agarwal_2025] 📄。（Part A 需 eGFR 40–90 並強制血壓監測，於首 50 名 Part A 受試者安全審查後，Part B 放寬至 eGFR 30–90 [confidence_trial_Green_2023][confidence_trial_Vaduganathan_2025] 📄。）

### 1.2 族群：一個「已被良好治療、殘餘 albuminuria 仍高」的真實世界世代 🟡

自 **2022/7 至 2024/8**，於 **14 國、143 站點**共隨機 **818 人** [confidence_baseline_Agarwal_2025_NDT] 📄。基線特徵刻畫出中重度、殘餘風險高的族群：平均 eGFR **54.2 ± 17.1 mL/min/1.73 m²**、中位 UACR **583（IQR 292–1140）mg/g**、平均 HbA1c **7.3 ± 1.2%**、平均血鉀 **4.48 ± 0.42 mmol/L**、25% 為女性 [confidence_baseline_Agarwal_2025_NDT] 📄。背景用藥近乎飽和——ACEi/ARB **788（98.4%）**、statin **313（39.1%）**、GLP-1RA **182（22.7%）**、利尿劑 **291（36.3%）**、beta-blocker **268（33.5%）**；共病 ASCVD **223（28%）**、心衰病史 **30（4%）** [confidence_baseline_Agarwal_2025_NDT] 📄。

**納入／排除的嚴格性決定了外推邊界**：納入 T2D、HbA1c <11%、eGFR 30–90、UACR 100–5000 mg/g、且已服最大耐受 ACEi/ARB >1 個月者；**排除**血鉀 >4.8 mmol/L、HFrEF 且有持續症狀、90 天內曾中風／心肌梗塞／因心衰惡化住院、T1D、腎移植，並要求篩選前 8 週內未用 SGLT2i 或鉀結合劑 [confidence_trial_Agarwal_2025] 📄。**臨床意涵**：這是一個血鉀「有空間」（≤4.8）、心衰不穩者被排除的族群——把 CONFIDENCE 的血鉀數字直接套到血鉀已偏高或不穩定心衰病人身上須保留。

### 1.3 終點階層：把「證得多硬」講清楚 🟡

- **Primary（主要療效終點）**：Day 180 時 log-transformed 平均 UACR 自基線的相對變化，含**兩個主要比較**（combination vs finerenone、combination vs empagliflozin），以 Holm–Bonferroni 法控制多重檢定 [confidence_trial_Agarwal_2025][confidence_trial_Green_2023] 📄。
- **Secondary**：停藥後（Day 180→210）UACR 相對變化（可逆性）、達到 30%／40%／50% UACR 下降門檻的比例、eGFR 變化、incident hyperkalemia [confidence_trial_Green_2023][confidence_trial_Agarwal_2025] 📄。
- **Prespecified 次分析**：KDIGO 風險分層（Vaduganathan）[confidence_trial_Vaduganathan_2025] 📄、血鉀時程與決定因子（JACC）[confidence_trial_Agarwal_2026] 📄。
- **Exploratory / post hoc**：eGFR 中介分析（JASN 的 causal mediation 明示為 exploratory）[confidence_egfr_mediation_Agarwal_2026] 📄。

分析族群：主要療效用 **Full Analysis Set**（所有隨機者，排除誤隨機與 GCP 重大違規站點），安全性用 **Safety Analysis Set**（隨機且至少服 1 劑）[confidence_trial_Green_2023][confidence_trial_Agarwal_2025] 📄。樣本數估算：每臂 226–228 名可達 80% power 偵測「combination 較任一單藥至少多降 20%」，計入約 15% 中止後目標約 269/臂 [confidence_trial_Green_2023][confidence_trial_Agarwal_2025] 📄。

**受試者流向（CONSORT 要點）**：**1664 人**篩選、**818 人**隨機（2022/6/23–2024/8/14），4 名誤隨機且未服藥、14 名來自一個 GCP 違規站點被排除 → **800 人**進入 FAS（combination 269、finerenone 264、empagliflozin 267）、**798 人**進入安全族群（268／264／266）、**746 人**完成 30 天追蹤 [confidence_trial_Agarwal_2025] 📄。

**表 1｜CONFIDENCE 設計速覽（供後續引用）**

| 面向 | 內容 | 來源 |
|---|---|---|
| 設計 | 隨機、雙盲、double-dummy、三臂平行、Phase 2 | `confidence_trial_Green_2023` 📄 |
| 療程 | 7.5–8.5 個月；停藥後 Day 210 追蹤 | `confidence_trial_Green_2023` 📄 |
| 分配 | 1:1:1；分層 eGFR(<60/≥60)、UACR(≤850/>850) | `confidence_trial_Agarwal_2025` 📄 |
| N | 篩 1664 → 隨機 818 → FAS 800 / 安全 798 | `confidence_trial_Agarwal_2025` 📄 |
| 族群 | eGFR 54.2±17.1、UACR 583、K 4.48、ACEi/ARB 98.4% | `confidence_baseline_Agarwal_2025_NDT` 📄 |
| Primary | Day 180 log-UACR 相對變化（2 個比較） | `confidence_trial_Agarwal_2025` 📄 |

---

## 2. 主要療效：同步起始的 albuminuria 益處是「over-additive」

### 2.1 主要結果 🟡

Day 180 時，combination 的 UACR 下降較 **finerenone 單藥多 29%**（least-squares mean ratio 0.71；95% CI 0.61–0.82；P<0.001）、較 **empagliflozin 單藥多 32%**（LSMR 0.68；95% CI 0.59–0.79；P<0.001），兩個主要比較均達統計顯著 [confidence_trial_Agarwal_2025] 📄。以自基線的絕對降幅表達：**combination 約 −52%、finerenone 約 −32%、empagliflozin 約 −29%**——作者明言 52% 與「finerenone 32% + empagliflozin 29% 的全加成預期」相符 [confidence_trial_Agarwal_2025] 📄。對應的自基線 LSMR（baseline→Day 180）為 combination **0.48（0.44–0.54）**、finerenone **0.68（0.61–0.76）**、empagliflozin **0.71（0.64–0.79）** [confidence_trial_Agarwal_2025] 📄。

> **「over-additive」的精確含義**：CONFIDENCE 的 52% 是**加成（additive）而非協同（synergy）**——它等於兩單藥效應之和，主文與 editorial 沿用的「over-additive」一詞係相對於「只加一藥」的增益，而非統計上超越加成模型。此細節見 [`statistical_insights_myths.md`](statistical_insights_myths.md)。

### 2.2 時間動態與可逆性 🟡

益處出現得很快：**Day 14 時 combination 的 UACR 已較基線降 >30%，Day 90 已 >40%** [confidence_trial_Agarwal_2025] 📄。停藥後（Day 180→Day 210）UACR 回升但方向可逆——回升的 LSMR（Day 180→210）為 combination **1.63（1.49–1.78）**、finerenone **1.45（1.32–1.59）**、empagliflozin **1.44（1.32–1.58）**，顯示效應為藥理性、於撤藥後部分回復 [confidence_trial_Agarwal_2025] 📄。

### 2.3 跨 KDIGO 風險層的一致性（Vaduganathan prespecified）🟡

在 **781 名有資料者**中，11.3% 為 low/moderate、29.6% high、**462（59.2%）very high risk** [confidence_trial_Vaduganathan_2025] 📄。combination 的 UACR 降幅**跨風險層一致**（low/mod **−61.7%**、high **−60.7%**、very high **−52.4%**），且各層皆優於任一單藥（monotherapy 對照：finerenone −48.1%／−40.6%／−34.3%；empagliflozin −38.3%／−28.1%／−36.2%）[confidence_trial_Vaduganathan_2025] 📄。以 very high risk 層（n=462）為例，combination vs finerenone LSMR **0.72（0.59–0.89）**、vs empagliflozin **0.75（0.61–0.91）**，且各風險層間 **P_interaction >.05** [confidence_trial_Vaduganathan_2025] 📄。達臨床有意義（>30% UACR 下降）者在 combination 各層皆過半（low/mod 58.1%〔18/31〕、high 74.2%、very high 70.6%〔101/143〕），P_interaction 0.27（vs finerenone）／0.43（vs empagliflozin）[confidence_trial_Vaduganathan_2025] 📄。**臨床意涵**：相對益處不因基線腎風險高低而改變，支持「不必等到極高風險才聯用」。

---

## 3. 機轉的解剖：急性 eGFR dip 與「非血流動力學」加成（JASN mediation）

這是對內分泌／腎臟科醫師最有價值的一層——combination 多出來的 albuminuria 益處，究竟來自「再壓一次球內壓（血流動力學）」還是「另一條抗纖維化通路」？

### 3.1 誰會急性 dip：baseline eGFR 高者、用利尿劑者 🟡

在 eGFR-mediation 分析（N=790：combination 265、finerenone 263、empagliflozin 262）中，急性 eGFR 變化定義為 baseline→Day 14 [confidence_egfr_mediation_Agarwal_2026] 📄。**急性下降的決定因子**：baseline eGFR 越高（P<0.001）、baseline 使用利尿劑者（P<0.001）下降越明顯；baseline SBP 僅邊緣（P≈0.05／0.053），baseline UACR 無顯著影響 [confidence_egfr_mediation_Agarwal_2026] 📄。以 logistic 迴歸量化「≥30% eGFR 下降」的勝算：**baseline eGFR 每高 10 mL/min，OR 1.24（1.11–1.39）**；**baseline 使用利尿劑 OR 1.96（1.32–2.91）** [confidence_egfr_mediation_Agarwal_2026] 📄。關鍵是**可逆**：撤藥後 eGFR 回升趨向基線，且在 baseline eGFR 30 者「未觀察到大而持續的下降」，提示晚期 CKD 的血流動力學反應鈍化 [confidence_egfr_mediation_Agarwal_2026] 📄。這與 CONFIDENCE 的 KDIGO 分層一致——combination 的 >30% eGFR 下降（Day 30±4）**反而集中在 low/moderate（12.1%）與 high（8.2%）風險層，very high 層最少（4.4%）**，因後者基線 eGFR 已低、可壓縮的 hyperfiltration 空間小 [confidence_trial_Vaduganathan_2025] 📄。

### 3.2 中介百分比：28% vs 5.2%（本節最重要）🟡

在 exploratory causal mediation 分析（N=690）中：**「把 empagliflozin 加到 finerenone 上」的 UACR 益處，急性 eGFR 變化中介 28%（P=0.07）**；而**「把 finerenone 加到 empagliflozin 上」的益處，急性 eGFR 變化僅中介 5.2%（P=0.23）** [confidence_egfr_mediation_Agarwal_2026] 📄。換言之，加 empagliflozin 的加成有相當部分走血流動力學（球內壓下修），而加 finerenone 的加成**幾乎全屬非血流動力學**——與其直接抗發炎／抗纖維化機轉一致，並有臨床前資料佐證（SGLT2 缺失可防高濾過卻不減腎纖維化／發炎標記）[confidence_egfr_mediation_Agarwal_2026] 📄。

急性 dip 與高血鉀在時間上「同行」：hyperkalemia 於全體 113/790（14%）出現，在**曾 ≥30% eGFR 下降者為 23%（31/133）**、未下降者為 **12%（82/657）**，此型態與所受治療無關 [confidence_egfr_mediation_Agarwal_2026] 📄。作者的臨床建議是把急性 dip 視為腎絲球「unloading」的預期訊號、先排除 NSAID／容量不足／利尿劑過量等外因再考慮停藥，並於起始後首 90 天監測 eGFR 與血鉀 [confidence_egfr_mediation_Agarwal_2026] 📄。

### 3.3 誠實邊界（mediation）🟡🔴

中介分析係 **exploratory**、CI 寬、兩個關鍵 P 值皆 >0.05（28% 的 P=0.07、5.2% 的 P=0.23），作者明示須謹慎解讀 [confidence_egfr_mediation_Agarwal_2026] 📄。因此「finerenone 加成主要非血流動力學」是**方向明確、機轉合理的推論**，而非統計確立的中介證明。

---

## 4. 血鉀：同步起始「並沒有」抵消 finerenone 的高血鉀（JACC，反直覺）

### 4.1 隨機化證據：no mitigation 🟡

CONFIDENCE 的血鉀 prespecified 次分析（以中央實驗室 K >5.5 mmol/L 定義 hyperkalemia，moderate 5.5–6.0、severe ≥6.0）給出反直覺結論：**combination 與 finerenone 單藥在血鉀平均變化（P=0.91）與發生高血鉀之 odds（P=0.85）均無顯著差異** [confidence_trial_Agarwal_2026] 📄。整體 hyperkalemia 113 人（14.5%）：**combination 40/265（15.1%）、finerenone 48/255（18.8%）、empagliflozin 25/259（9.7%）** [confidence_trial_Agarwal_2026] 📄。血鉀上升最大出現在 Day 14（combination 與 finerenone 約 0.2 與 0.25 mmol/L），其後穩定並於停藥後回落 [confidence_trial_Agarwal_2026] 📄。Sinclair 的 editorial 全文定性轉述最清楚：隨機分入 combination 者的血鉀上升與高血鉀風險「和分入 finerenone 單藥者相似」，顯示同步起始並不能防止 MRA 介導的高血鉀 [hyperkalemia_combo_Sinclair_2026] 📄。

> **注意兩套數字不可混用**：NEJM 主文以「investigator-reported」計 hyperkalemia（combination 9.3%、finerenone 11.4%、empagliflozin 3.8%，安全族群 Table 3）[confidence_trial_Agarwal_2025] 📄；JACC 次分析以「中央實驗室 K >5.5」計（15.1%／18.8%／9.7%）[confidence_trial_Agarwal_2026] 📄；Cheng editorial 引用的 15.3% vs 18.6% 亦屬另一切分 [combination_editorial_Cheng_2025] 📄。三者定義不同、分母不同，比較時須標明來源。無論用哪套，方向一致：**combination 相對 finerenone 僅數值略低、未被統計上抵消**。

### 4.2 決定因子與臨床後果 🟡

高血鉀的決定因子由 logistic 迴歸量化：**baseline 血鉀每高 1 mmol/L，aOR 9.23（5.07–16.81）**；**eGFR 每低 5 mL/min/1.73 m²，aOR 1.11（1.03–1.20）** [confidence_trial_Agarwal_2026] 📄。相對 empagliflozin 單藥，combination 的 aOR 為 **2.69（1.46–4.96）**、finerenone 的 aOR 為 **2.56（1.42–4.59）**，而 combination vs finerenone 無顯著差異（P=0.85）[confidence_trial_Agarwal_2026] 📄。臨床上重要的是**後果輕微**：NEJM 主文載**僅 3 名（每臂 1 名）因高血鉀永久停藥**，且 AKI 在 combination 僅 1.9% [confidence_trial_Agarwal_2025] 📄。

### 4.3 高血鉀不在療效的因果路徑上 🟡

血鉀曾被懷疑是「target engagement」的標記（即療效靠升鉀）。CONFIDENCE 的中介分析否定此說：**hyperkalemia 不在 UACR 下降的因果路徑上**，finerenone vs combination 的 UACR 益處經高血鉀中介的比例僅 **0.2%**，療效不因是否發生高血鉀而改變 [confidence_trial_Agarwal_2026] 📄。**意義**：這消除了「療效靠血鉀升高」的疑慮，但同時也拿掉了「SGLT2i 讓 finerenone 更安全」的短期證據。

### 4.4 為何矛盾？時序假說（Sinclair × FIVE-STAR）🔴

CONFIDENCE 的「同步不降鉀」與觀察性資料的「SGLT2i 降鉀」如何調和？Sinclair 提出**時序假說**：在 FIVE-STAR 次分析中，對**已慢性使用 SGLT2i** 者再加 finerenone，血鉀僅升 **0.13 mEq/L**，遠低於未用 SGLT2i 者的 **0.37 mEq/L（P-interaction 0.02）**；同一分析中 finerenone 整體使血鉀升 0.22 mEq/L、並較 placebo 多降 UACR 29%（24 週）[hyperkalemia_combo_Sinclair_2026] 📄。機轉推測為 SGLT2i 需時間誘導遠端小管鉀處理的適應（臨床前 dapagliflozin 保留近端 Kcnk1 表現）；同步起始時 finerenone 的升鉀在 SGLT2i「適應」建立前就發生，故無法被抵消 [hyperkalemia_combo_Sinclair_2026] 📄。Sinclair 因此呼籲一個直接的三臂 sequencing RCT（finerenone-first／同步／SGLT2i-first），以 finerenone 起始後的血鉀變化為主要終點 [hyperkalemia_combo_Sinclair_2026] 📄。

> **誠實邊界**：FIVE-STAR 的 SGLT2i 使用**非隨機化**（存在 confounding by indication，已用 SGLT2i 者本就耐受性較佳），CONFIDENCE 才是唯一無此偏誤的隨機設計 [hyperkalemia_combo_Sinclair_2026] 📄。故「SGLT2i 先行較安全」目前為 **hypothesis-generating** 🔴。FIDELITY 全文的方向性旁證：慢性 SGLT2i 背景下，實驗室確認 K >5.5 於 SGLT2i-only 子組較低（finerenone 臂 7.9% vs 無 SGLT2i/GLP-1RA 17.7%）[hyperkalemia_combo_Singh_2026] 📄——但同屬非隨機次組。

---

## 5. 安全綜覽（供臨床引用）

**表 2｜CONFIDENCE 三臂安全對照**

| 安全指標 | Combination | Finerenone | Empagliflozin | 來源 |
|---|---|---|---|---|
| Hyperkalemia（investigator，安全族群） | 25（9.3%） | 30（11.4%） | 10（3.8%） | `confidence_trial_Agarwal_2025` 📄 |
| Hyperkalemia（中央實驗室 K>5.5） | 40/265（15.1%） | 48/255（18.8%） | 25/259（9.7%） | `confidence_trial_Agarwal_2026` 📄 |
| >30% eGFR 下降（Day 30） | 17（6.3%） | 10（3.8%） | 3（1.1%） | `confidence_trial_Agarwal_2025` 📄 |
| 嚴重不良事件（SAE） | 19/268（7.1%） | 16/264（6.1%） | 17/266（6.4%） | `confidence_trial_Agarwal_2025` 📄 |
| 因高血鉀永久停藥 | 1 | 1 | 1 | `confidence_trial_Agarwal_2025` 📄 |
| 急性腎損傷（AKI） | 1.9% | 罕見 | 罕見 | `confidence_trial_Agarwal_2025` 📄 |
| 症狀性低血壓 | 3 名（整體 combination） | 罕見 | 罕見 | `combination_editorial_Cheng_2025` 📄 |
| 死亡（治療起始後） | 3 | 0 | 3 | `confidence_trial_Agarwal_2025` 📄 |

任一組因不良事件永久停藥皆 <5%（整體 30 名，3.8%）[confidence_trial_Agarwal_2025] 📄。Vaduganathan 補充：symptomatic hypotension 於 low/moderate 與 high 風險層無人發生、僅 very high 層 2 名；investigator-reported AKI 各層 ≤3% [confidence_trial_Vaduganathan_2025] 📄。**判讀重點**：>30% eGFR 下降是血流動力學可逆現象、非腎損傷，且最大者恰是基線腎功能最好、最禁得起的族群，不應觸發停藥（機轉對讀見 §3.1 與 egfr_dip 專章）。

---

## 6. surrogate 的橋樑與 hard-outcome 缺口

### 6.1 為何用 UACR、以及它能撐多遠 🟡

CONFIDENCE 的主終點是 UACR，不是 kidney failure。理由是可行性：一個為偵測硬腎終點差異而 power 的 Phase 3 試驗，估計需隨機化**約 41,000 人**，可預見的未來不會有 [combination_editorial_Georgianos_2025] 📄。而 UACR 是硬腎益處的主要中介——**2019 年 41 試驗、29,979 人 patient-level 統合**顯示，前 6 個月 **≥30% albuminuria 下降對應長期複合腎終點風險降 27%（HR 0.73；95% CI 0.67–0.81）**，在高基線 albuminuria 者更強 [combination_editorial_Georgianos_2025] 📄。CONFIDENCE 過半受試者在各風險層達到此門檻 [confidence_trial_Vaduganathan_2025] 📄，故 Georgianos 主張「改變日常實務的時機就是現在」[combination_editorial_Georgianos_2025] 📄。

### 6.2 保留方：硬終點的 additivity 仍未證實 🔴

UACR 終究是 surrogate。Wen 統合指出，相較 **SGLT2i 單藥**，combination 在 mortality、MACE、MAKE 上**均無顯著額外益處**（OR 0.73〔0.47–1.13；p=0.16〕、0.77〔0.55–1.08；p=0.14〕、0.87〔0.58–1.31；p=0.51〕），且 trial sequential analysis 顯示尚未越過 monitoring boundary、仍需足夠 power 的 RCT [hyperkalemia_combo_Wen_2026] 📄。相對 **finerenone 單藥**，combination 於高血鉀無顯著增加（OR 1.09；95% CI 0.52–2.28；p=0.8252；I²=95.1%），UACR 多降約 10%（mean difference 0.10；0.00–0.19；p=0.045）[hyperkalemia_combo_Wen_2026] 📄。**整合**：combination 相對 finerenone「多降 UACR、血鉀不惡化」→ 傾向支持；相對 SGLT2i「硬終點益處未證實、血鉀顯著惡化（OR 3.00；2.50–3.61）」→ 須保留 [hyperkalemia_combo_Wen_2026] 📄。

---

## 7. 誠實邊界（Evidence limits）🟡🔴

- **surrogate**：主終點為 UACR、療程僅 **180 天**，無 hard renal/CV outcome，長期硬終點屬 under-ascertained 🟡🔴 [confidence_trial_Agarwal_2025][hyperkalemia_combo_Wen_2026]。
- **單一 Phase 2 試驗**：CONFIDENCE 為單一、嚴格納入的 Phase 2；血鉀 ≤4.8、心衰不穩者被排除，對更廣族群的成本效益與安全性未知 🔴 [confidence_trial_Vaduganathan_2025]。
- **中介分析為 exploratory**：28% 與 5.2% 的中介百分比 CI 寬、P>0.05，屬機轉推論而非統計證明 🟡 [confidence_egfr_mediation_Agarwal_2026]。
- **時序假說未經隨機化驗證**：「SGLT2i 先行降鉀較佳」源自非隨機的 FIVE-STAR 次分析與臨床前資料，待專門 sequencing RCT 🔴 [hyperkalemia_combo_Sinclair_2026]。
- **數字專屬其原始族群**：具體效應量屬 CONFIDENCE 世代（eGFR 30–90、UACR 100–5000、T2D、已服 RASi），外推至非糖尿病 CKD、HFrEF、血鉀偏高者須保留 🔴。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|------|------|------------------|
| 同步起始 UACR over-additive（多降 29%／32%，P<0.001） | 🟡 surrogate RCT | `confidence_trial_Agarwal_2025` 📄 |
| 益處跨 KDIGO 風險層一致（P_interaction >.05） | 🟡 prespecified | `confidence_trial_Vaduganathan_2025` 📄 |
| 加 finerenone 的加成幾乎非血流動力學（中介 5.2%） | 🟡 exploratory | `confidence_egfr_mediation_Agarwal_2026` 📄 |
| 同步起始不抵消 finerenone 高血鉀（P=0.91／0.85） | 🟡 prespecified | `confidence_trial_Agarwal_2026` 📄 |
| 高血鉀不在 UACR 下降的因果路徑（中介 0.2%） | 🟡 exploratory | `confidence_trial_Agarwal_2026` 📄 |
| >30% eGFR dip 可逆、集中於低風險層 | 🟡 | `confidence_trial_Vaduganathan_2025`／`confidence_egfr_mediation_Agarwal_2026` 📄 |
| UACR→硬腎終點的橋樑（≥30% 降→27% 風險降） | 🟡 trial-level meta | `combination_editorial_Georgianos_2025` 📄 |
| combination vs SGLT2i 硬終點 additivity | 🔴 未證實 | `hyperkalemia_combo_Wen_2026` 📄 |
| SGLT2i 先行降鉀之時序假說 | 🔴 hypothesis | `hyperkalemia_combo_Sinclair_2026` 📄 |
| 同步起始之 hard-outcome RCT | 🔴 尚無（誠實揭露） | —（估計需約 41,000 人）`combination_editorial_Georgianos_2025` 📄 |

## 本地全文語料（可 grep 稽核）

📄 全文：`confidence_trial_Green_2023`（設計）、`confidence_baseline_Agarwal_2025_NDT`（基線）、`confidence_trial_Agarwal_2025`（NEJM 主文）、`confidence_egfr_mediation_Agarwal_2026`（JASN eGFR 中介）、`confidence_trial_Agarwal_2026`（JACC 高血鉀次分析）、`confidence_trial_Vaduganathan_2025`（KDIGO 風險分層）、`combination_editorial_Georgianos_2025`（editorial）、`combination_editorial_Cheng_2025`（pillar risk-based narrative review）、`hyperkalemia_combo_Sinclair_2026`（時序假說 editorial）、`hyperkalemia_combo_Wen_2026`（統合分析）、`hyperkalemia_combo_Singh_2026`（FIDELITY 三藥旁證）。

---

## References（Vancouver + 本地檔名）

1. Green JB, Mottl AK, Bakris G, et al. Design of the COmbinatioN effect of FInerenone anD EmpaglifloziN in participants with chronic kidney disease and type 2 diabetes using a UACR Endpoint study (CONFIDENCE). Nephrol Dial Transplant. 2023;38(4):894–903. doi:10.1093/ndt/gfac198. 📄 [confidence_trial_Green_2023]
2. Agarwal R, Green JB, Heerspink HJL, et al. Finerenone with empagliflozin in chronic kidney disease and type 2 diabetes (CONFIDENCE). N Engl J Med. 2025;393(6):533–543. doi:10.1056/NEJMoa2410659. 📄 [confidence_trial_Agarwal_2025]
3. Agarwal R, Green JB, Heerspink HJL, et al. CONFIDENCE trial: baseline clinical characteristics. Nephrol Dial Transplant. 2025;40(8):1559–1569. doi:10.1093/ndt/gfaf022. 📄 [confidence_baseline_Agarwal_2025_NDT]
4. Agarwal R, Correa-Rotter R, Navaneethan SD, et al. Acute eGFR changes and their mediation of albuminuria reduction with empagliflozin and finerenone (CONFIDENCE). J Am Soc Nephrol. 2026. doi:10.1681/ASN.0000001071. 📄 [confidence_egfr_mediation_Agarwal_2026]
5. Agarwal R, Green JB, Heerspink HJL, et al. Risk of hyperkalemia with empagliflozin, finerenone, or both: secondary analysis of the CONFIDENCE randomized trial. J Am Coll Cardiol. 2026;87(7):772–784. doi:10.1016/j.jacc.2025.10.049. 📄 [confidence_trial_Agarwal_2026]
6. Vaduganathan M, Green JB, Heerspink HJL, et al. Simultaneous initiation of finerenone and empagliflozin across the spectrum of kidney risk in the CONFIDENCE trial. Nephrol Dial Transplant. 2026;41(1):161–170. doi:10.1093/ndt/gfaf160. 📄 [confidence_trial_Vaduganathan_2025]
7. Georgianos PI, Koufakis T, Arampatzis S, Liakopoulos V. CONFIDENCE in the safety and efficacy of dual therapy with an SGLT-2 inhibitor and finerenone in patients with chronic kidney disease and type 2 diabetes. Diabetes Obes Metab. 2025;27(11):6097–6100. doi:10.1111/dom.70026. 📄 [combination_editorial_Georgianos_2025]
8. Cheng AYY, Mottl A, Magwire M. Pillar risk-based treatment for chronic kidney disease in people with type 2 diabetes: a narrative review. Diabetes Ther. 2025;16(11):2083–2099. doi:10.1007/s13300-025-01796-7. 📄 [combination_editorial_Cheng_2025]
9. Sinclair MR, Edmonston D. It's about time: potassium risk with combination guideline-directed medical therapy. Kidney Int Rep. 2026;11:106609. doi:10.1016/j.ekir.2026.106609. 📄 [hyperkalemia_combo_Sinclair_2026]
10. Wen CF, Chuang MH, Wu VC, Chen JY. Efficacy of combined SGLT2 inhibitors and finerenone in chronic kidney disease: a systematic review and meta-analysis. Front Pharmacol. 2026;17:1803971. doi:10.3389/fphar.2026.1803971. 📄 [hyperkalemia_combo_Wen_2026]
11. Singh AK, Anker SD, Pitt B, et al. A FIDELITY analysis on finerenone with SGLT-2i and GLP-1RA in CKD. Kidney Int Rep. 2026. doi:10.1016/j.ekir.2025.10.032. 📄 [hyperkalemia_combo_Singh_2026]

---

*此檔為主題三之延伸拆解，撰寫日期基準 2026-07-12。所有具體數字均可 grep 回上列本地全文 MD。CONFIDENCE 的療效結論屬 surrogate（UACR）／180 天／單一 Phase 2；「同步不抵消高血鉀」為隨機化證據（穩健），「SGLT2i 先行降鉀」與「combination 相對 SGLT2i 硬終點 additivity」則分屬 hypothesis 與未證實，已明示邊界。*
