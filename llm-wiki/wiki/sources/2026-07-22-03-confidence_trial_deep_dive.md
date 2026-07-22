---
tags: [素材摘要, CONFIDENCE, 試驗設計, 高血鉀, 中介分析]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/03-confidence_trial_deep_dive.md
images: 0
image_paths: []
---

# CONFIDENCE 深度解析 · 第一個直接檢驗「同步起始」的三臂試驗

> CONFIDENCE 在 albuminuria 這個替代終點上給了乾淨、over-additive 的答案，卻同時戳破「同步加 SGLT2i 能抵消 finerenone 高血鉀」的流行假說；而所有 hard renal/CV outcome 的優劣，它沒有、也無力回答。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/03-confidence_trial_deep_dive.md
- **消化日期**：2026-07-22

## 核心觀點

1. **設計「乾淨」在哪裡（🟡）**：NCT05254002，隨機、雙盲、**double-dummy**、國際多中心、三臂平行、**Phase 2**，每位受試者療程 7.5–8.5 個月。1:1:1 分入 (i) finerenone 10/20 mg + empagliflozin 10 mg；(ii) finerenone + empagliflozin-matching placebo；(iii) empagliflozin 10 mg + finerenone-matching placebo。double-dummy 讓單藥臂也吞下對應安慰劑，是全盲與無偏比較的設計核心。finerenone 起始劑量依 baseline eGFR（≥60 起始 20 mg、<60 起始 10 mg），Day 30 後若血鉀 ≤4.8 且 eGFR 下降 <30% 可上調至 20 mg。隨機化依 eGFR（<60 vs ≥60）與 UACR（≤850 vs >850 mg/g）分層。訪視 Day 14、30、90、180，停藥後 Day 210 再測一次評估可逆性。Part A 需 eGFR 40–90，安全審查後 Part B 放寬至 30–90。

2. **族群（🟡）**：2022/7–2024/8，14 國、143 站點、隨機 **818 人**。基線 mean eGFR **54.2 ± 17.1**、中位 UACR **583（IQR 292–1140）mg/g**、HbA1c **7.3 ± 1.2%**、血鉀 **4.48 ± 0.42 mmol/L**、25% 女性。背景用藥近飽和：ACEi/ARB **788（98.4%）**、statin **313（39.1%）**、GLP-1RA **182（22.7%）**、利尿劑 **291（36.3%）**、beta-blocker **268（33.5%）**；ASCVD **223（28%）**、心衰病史 **30（4%）**。**關鍵排除**：血鉀 >4.8、HFrEF 有持續症狀、90 天內中風／MI／因心衰住院、T1D、腎移植、篩選前 8 週內用過 SGLT2i 或鉀結合劑。

3. **終點階層**：**Primary** = Day 180 log-transformed 平均 UACR 自基線相對變化，含兩個主要比較（combo vs finerenone、combo vs empagliflozin），以 Holm–Bonferroni 控制多重檢定。**Secondary** = 停藥後（Day 180→210）UACR 變化、達 30%/40%/50% UACR 下降的比例、eGFR 變化、incident hyperkalemia。**Prespecified 次分析** = KDIGO 風險分層（Vaduganathan）、血鉀時程與決定因子（JACC）。**Exploratory** = eGFR 中介分析（JASN，明示為 exploratory）。

4. **CONSORT 流向**：篩選 **1664** → 隨機 **818**（2022/6/23–2024/8/14）→ 排除 4 名誤隨機未服藥、14 名 GCP 違規站點 → FAS **800**（combination 269、finerenone 264、empagliflozin 267）、安全族群 **798**（268／264／266）、完成 30 天追蹤 **746**。樣本數估算：每臂 226–228 名可達 80% power 偵測「combination 較任一單藥至少多降 20%」，計入約 15% 中止後目標約 269/臂。

5. **主要療效（🟡）**：combo 較 finerenone 多降 **29%**（LSMR 0.71；0.61–0.82；P<0.001）、較 empagliflozin 多降 **32%**（0.68；0.59–0.79；P<0.001）。自基線降幅 combo 約 −52%、finerenone 約 −32%、empagliflozin 約 −29%；自基線 LSMR 為 0.48（0.44–0.54）／0.68（0.61–0.76）／0.71（0.64–0.79）。時間動態：**Day 14 combo UACR 已較基線降 >30%、Day 90 已 >40%**；停藥回升 LSMR 1.63／1.45／1.44。

6. **跨 KDIGO 風險層一致（🟡 prespecified）**：781 名有資料者中 11.3% low/moderate、29.6% high、**462（59.2%）very high**。combo 降幅 low/mod **−61.7%**、high **−60.7%**、very high **−52.4%**，各層皆優於單藥（finerenone −48.1%／−40.6%／−34.3%；empagliflozin −38.3%／−28.1%／−36.2%）。very high 層（n=462）combo vs finerenone LSMR **0.72（0.59–0.89）**、vs empagliflozin **0.75（0.61–0.91）**，各層 P_interaction >.05。>30% UACR 下降者在 combo 各層皆過半（low/mod 58.1%〔18/31〕、high 74.2%、very high 70.6%〔101/143〕）。

7. **誰會急性 dip（🟡）**：mediation 分析 N=790（combination 265、finerenone 263、empagliflozin 262）。決定因子為 baseline eGFR 越高（P<0.001）、baseline 使用利尿劑（P<0.001）；baseline SBP 僅邊緣（P≈0.05/0.053）、baseline UACR 無顯著影響。logistic 量化「≥30% eGFR 下降」：baseline eGFR 每高 10 mL/min **OR 1.24（1.11–1.39）**、baseline 使用利尿劑 **OR 1.96（1.32–2.91）**。

8. **中介百分比 28% vs 5.2%（🟡 exploratory，N=690）**：加 empagliflozin 的益處經急性 eGFR 中介 **28%（P=0.07）**；加 finerenone 的益處僅中介 **5.2%（P=0.23）**。急性 dip 與高血鉀「同行」：hyperkalemia 全體 113/790（14%），在曾 ≥30% eGFR 下降者 **23%（31/133）**、未下降者 **12%（82/657）**，此型態與所受治療無關。作者建議把急性 dip 視為腎絲球 unloading 的預期訊號，先排除 NSAID／容量不足／利尿劑過量再考慮停藥，並於起始後首 90 天監測 eGFR 與血鉀。

9. **血鉀反直覺結果（🟡 prespecified）**：以中央實驗室 K >5.5 定義（moderate 5.5–6.0、severe ≥6.0），**combination 與 finerenone 單藥在血鉀平均變化（P=0.91）與高血鉀 odds（P=0.85）均無顯著差異**。整體 113 人（14.5%）：combination **40/265（15.1%）**、finerenone **48/255（18.8%）**、empagliflozin **25/259（9.7%）**。血鉀上升最大在 Day 14（combination 與 finerenone 約 0.2 與 0.25 mmol/L），其後穩定、停藥後回落。**三套數字不可混用**：NEJM 主文 investigator-reported 為 9.3%／11.4%／3.8%；JACC 中央實驗室為 15.1%／18.8%／9.7%；Cheng editorial 引 15.3% vs 18.6%——定義與分母不同。

10. **高血鉀決定因子與後果**：baseline 血鉀每高 1 mmol/L **aOR 9.23（5.07–16.81）**；eGFR 每低 5 mL/min **aOR 1.11（1.03–1.20）**。相對 empagliflozin 單藥，combination **aOR 2.69（1.46–4.96）**、finerenone **aOR 2.56（1.42–4.59）**，兩者間 P=0.85。後果輕微：僅 **3 名（每臂 1 名）因高血鉀永久停藥**、AKI combination 1.9%。且 **hyperkalemia 不在 UACR 下降的因果路徑上——percent mediation 僅 0.2%**。

11. **時序假說（🔴）**：FIVE-STAR 次分析中，已慢性使用 SGLT2i 者再加 finerenone 血鉀僅升 **0.13 mEq/L**，未用者升 **0.37 mEq/L（P-interaction 0.02）**；同一分析中 finerenone 整體升鉀 0.22 mEq/L、24 週較 placebo 多降 UACR 29%。機轉推測為 SGLT2i 需時間誘導遠端小管鉀處理適應（臨床前 dapagliflozin 保留近端 Kcnk1）。FIVE-STAR 的 SGLT2i 使用非隨機化，屬 hypothesis-generating。

12. **安全綜覽**：SAE combination 19/268（7.1%）、finerenone 16/264（6.1%）、empagliflozin 17/266（6.4%）；因不良事件永久停藥整體 30 名（3.8%）、各組 <5%；死亡（治療起始後）3／0／3；symptomatic hypotension 於 low/moderate 與 high 層無人發生、僅 very high 層 2 名。

13. **surrogate 橋樑與 hard-outcome 缺口**：硬終點 Phase 3 估計需隨機化約 **41,000 人**；2019 年 41 試驗、29,979 人 patient-level 統合顯示前 6 個月 ≥30% albuminuria 下降對應長期複合腎終點風險降 **27%（HR 0.73；0.67–0.81）**。保留方 Wen：相對 SGLT2i 單藥，combination mortality OR 0.73（0.47–1.13；p=0.16）、MACE 0.77（0.55–1.08；p=0.14）、MAKE 0.87（0.58–1.31；p=0.51）皆不顯著；相對 finerenone 單藥高血鉀 OR 1.09（0.52–2.28；p=0.8252；I²=95.1%）、UACR 多降約 10%（mean difference 0.10；0.00–0.19；p=0.045）。

## 關鍵概念

[[CONFIDENCE]]、[[CONFIDENCE]]、[[Finerenone]]、[[Empagliflozin]]、[[高血鉀]]、[[eGFR dip]]、[[eGFR×UACR 風險分層]]、[[中介分析]]、[[FIVE-STAR]]、[[中介分析]]、[[替代終點]]

## 與其他素材的關聯

- 主文 §2 的學術完整版 → [[2026-07-22-03-03_fourth_pillar_or_early_combination]]
- over-additive 的機制拆解與停藥反彈 → [[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]
- 三大爭議的完整對讀 → [[2026-07-22-03-discussion_controversies_endpoint_hyperkalemia_cost]]
- 統計陷阱（P 值沉默、超加成未檢定） → [[2026-07-22-03-statistical_insights_myths]]
- 急性 eGFR dip 的跨 class 對讀屬主題五 <!-- confidence: INFERRED -->

## 原文精彩摘錄

> **double-dummy 是關鍵**：它讓「單藥」臂也吞下對應的安慰劑，使投藥者、病人、結果評估者對分組全盲，是本試驗能對「同步起始」做出無偏比較的設計核心。

> 血鉀曾被懷疑是「target engagement」的標記（即療效靠升鉀）。CONFIDENCE 的中介分析否定此說：**hyperkalemia 不在 UACR 下降的因果路徑上**，經高血鉀中介的比例僅 **0.2%**。

> **判讀重點**：>30% eGFR 下降是血流動力學可逆現象、非腎損傷，且最大者恰是基線腎功能最好、最禁得起的族群，不應觸發停藥。

## 相關頁面

- [[2026-07-22-03-03_fourth_pillar_or_early_combination]]
- [[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]
- [[2026-07-22-03-discussion_controversies_endpoint_hyperkalemia_cost]]
- [[2026-07-22-03-statistical_insights_myths]]
- [[2026-07-22-03-background_guideline_placement_four_pillars]]
