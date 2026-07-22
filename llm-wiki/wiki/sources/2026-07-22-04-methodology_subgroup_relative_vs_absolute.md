---
tags: [素材摘要, 次族群方法學, 交互作用檢定, ICEMAN, 效果修飾]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/04-methodology_subgroup_relative_vs_absolute.md
images: 0
image_paths: []
---

# 方法學對讀 · 相對 vs 絕對、multiplicity、可信度評估與風險基礎 HTE

> 多數 subgroup 資料的用途是「校準臨床判讀」而非「重寫 eligibility」；「各亞群一致」必須被翻譯成「絕對受益隨基線風險放大」，不能被誤講成「人人同樣受益」。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/04-methodology_subgroup_relative_vs_absolute.md
- **消化日期**：2026-07-22

## 核心觀點

1. **相對 vs 絕對：為什麼「各組一樣」反而保證「絕對受益不一樣」**🟢。藥效有兩種講法——「打幾折（相對效果／HR）」和「省多少錢（絕對效果／ARR）」。相對效果通常跨風險穩定，但同樣打七折，本來風險高的人省下的絕對數字大得多。Sun 2010 把這件事講成一條定理：**若已知預後因子能定義不同風險組、而相對效果無異質性，則絕對效果的 subgroup effect 就「必然存在」**📄。statin 範例：相對降 **29.2%** 一致，10 年基線風險 5% 者 ARR 僅 **1.5%**、50% 者 ARR 達 **14.6%**——同一 RRR，ARR 差近 10 倍。

2. **套回 finerenone**：Agarwal 2023 的 eGFR×UACR 交互 **P=0.66**、Bakris 2023 的 P_interaction **0.62/0.67**、Neves 2026 的各 P_interaction **0.61–0.75**——這些「不顯著的交互」正是絕對受益梯度的**保證書**，而非「人人一樣」的證據📄。這是全主題的方法學樞紐。

3. **Multiplicity 與「方向相反」交互的稀有性**🟢。一個試驗切十幾個亞群做檢定，總有幾個「看起來有差」純屬運氣。真正該擔心的不是「程度差一點」，而是「方向相反」——而後者非常罕見。Yusuf 1991：量化交互（程度差異）常見且多為真；**質化交互（方向相反）罕見且多為假**；GISSI 的鏈激酶「只在前壁 MI、<65 歲、<6 小時有效」後被證明是 power 不足造成的假象📄。

4. **對 finerenone 的直接啟示**。華人／亞洲心血管終點「不顯著」、華人 FIGARO 非致死 MI **HR 4.75（CI 0.55–40.75）** 這類極端點估計，幾乎確定是**小樣本雜訊**，不該被解讀為「finerenone 對華人心臟無效或有害」；整體 CV HR 0.86 才是這些亞群更可靠的方向指引📄。

5. **Assmann 2000 與 Wallach 2017**🟢。Assmann 2000：多數試驗呈現 subgroup 卻**缺乏適當的交互檢定**、且過度強調 subgroup，應事前擬定 baseline 資料分析計畫📄。Wallach 2017：64 個 RCT 摘要中 **117 項** subgroup 宣稱，僅 **39.3%** 有顯著交互支持；其中僅 **34.8%** 有分層隨機、**28.3%** 事前設定、**僅 2.2% 校正多重比較**；曾被嘗試重現的 5 項**全部無法重現、效果量向虛無收斂**📄。這是對「publication layering（層層堆疊的次分析論文）」最有力的警示。

6. **ICEMAN 與可信度準則**🟢。Schandelmaier 2020 的 ICEMAN 工具（RCT 5 題、統合分析 8 題核心問項＋視覺類比信度評分）指出約 **14–26%** 的 RCT／統合分析會在摘要或討論強調至少一項效果修飾，而「錯誤宣稱的根本原因是機率（chance）」——即使真實效果對所有病人相同，檢驗夠多候選變項必然出現表面上的效果修飾📄。

7. **用 ICEMAN 精神稽核 finerenone 的兩個訊號**：**LVH×HHF（P=0.0024）** 方向合理（MR 活化與 LVH 相關）但事後、ECG 無中央裁決、未校正多重性 → **中低可信**，列 hypothesis-generating📄；**亞洲×腎臟（P=0.0009–0.0493）** 方向合理（鈉敏感／高鹽機轉）、跨多獨立分析一致，但華人單獨 P_interaction 不顯著 → **較高，但仍屬「校準」而非「重寫適應症」**📄。

8. **風險基礎 HTE 比單變量 subgroup 更貼近門診**🟢。Kent 2016（32 個大型試驗、39 分析）：試驗族群內結果風險有巨大異質性（極端四分位風險比 **EQRR 中位 4.3、最高 50.7**），**多數病人的風險低於試驗平均值**；在 18 個整體顯著的比較中，只有 1 個在比例尺度上有顯著的「治療×基線風險」交互，但**極端風險四分位間的絕對風險下降差異中位 5.1%、四分之一試驗超過 10%**📄。Kent 2018（PATH statement）主張以「reference class forecasting／多變量風險模型」取代單一變量 subgroup📄。

9. **整合結論與檢查清單**。與其逐一問「亞洲人？stage 4？有心衰？」，不如以 **eGFR × UACR（±HF 病史、±LVH）構成的多維風險**估個別病人的基線絕對事件率，再乘上穩定的相對效果（CV ~14%、腎臟 ~23%）得個人化 ARR/NNT——這就是從 average treatment effect 走向 precision-layered 判讀的操作定義。原文並附一頁「次族群判讀檢查清單」（八問：事前設定？分層隨機？校正多重比較？交互檢定顯著？方向為量化？有機轉理由？跨多獨立資料一致？整體結果穩健？）。

10. **穩健性補充（僅摘要）**📌🟡。Zuin 2026 對 finerenone 心血管結果做 fragility 分析（納入 FIDELIO、FIGARO、FIDELITY），本檔已知 FIDELIO 主要複合 CV **NNT 56**；fragility index 細節未取得，故**不對其穩健性作具體斷言**📌。

## 關鍵概念

[[交互作用檢定]]、[[絕對風險差]]、[[NNT]]、[[治療效應異質性]]、[[ICEMAN]]、[[多重比較校正]]、[[交互作用檢定]]、[[風險基礎 HTE]]、[[交互作用檢定]]、[[fragility index]]

## 與其他素材的關聯

- 本檔為 [[2026-07-22-04-04_who_gets_greatest_benefit]] §6 的延伸拆解，是全主題的方法學樞紐。
- statin 29.2%／ARR 1.5% vs 14.6% 的教學數字與 [[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]] 第 1 節共用同一來源。
- 本檔明示與 [[2026-07-22-04-statistical_insights_myths]] 分工互補：本檔處理相對／絕對、multiplicity、ICEMAN、risk-based HTE；姊妹檔處理 NNT 三缺陷、ITT vs on-treatment、競爭風險、PH 失效、fragility index。
- 「亞洲×腎臟」與「LVH×HHF」兩個受稽核的訊號分別來自 [[2026-07-22-04-cluster2_asian_chinese_japanese_subgroup]] 與 [[2026-07-22-04-cluster3_hf_lvh_targets_insulin_resistance]]。
- Kent 2018 的多變量風險模型主張若落實，將改變 [[2026-07-22-04-slides_figures_forest_heatmap_nnt]] 圖 2 森林圖的呈現方式。<!-- confidence: INFERRED -->

## 原文精彩摘錄

> **先用白話講**：藥物的效果有兩種講法——「打幾折（相對效果／HR）」和「省多少錢（絕對效果／ARR）」……所以「各亞群 HR 一樣」不是「人人受益一樣」，恰恰相反——它**保證**了高風險族群的絕對受益更大。

> 一個試驗切出十幾個亞群、每個都做檢定，總會有幾個「看起來有差」純粹是運氣。真正該擔心的不是「程度差一點」，而是「方向相反」（某亞群反而有害）——而後者其實**非常罕見**。

> 即使真實效果對所有病人相同，檢驗夠多候選變項必然出現表面上的效果修飾。

## 相關頁面
