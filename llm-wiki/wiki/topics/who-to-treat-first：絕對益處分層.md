---
tags: [主題, 絕對風險, NNT, 臨床分層]
created: 2026-07-22
updated: 2026-07-22
sources: [wiki/sources/2026-07-22-04-04_who_gets_greatest_benefit.md, wiki/sources/2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient.md, wiki/sources/2026-07-22-04-cluster2_asian_chinese_japanese_subgroup.md, wiki/sources/2026-07-22-04-cluster3_hf_lvh_targets_insulin_resistance.md, wiki/sources/2026-07-22-04-slides_figures_forest_heatmap_nnt.md, wiki/sources/2026-07-22-04-methodology_subgroup_relative_vs_absolute.md, wiki/sources/2026-07-22-04-statistical_insights_myths.md, wiki/sources/2026-07-22-01-statistical_insights_myths.md]
---

# who-to-treat-first：絕對益處分層

> 回應 purpose.md 關鍵問題四的核心：把「誰相對受益最大」換成「誰絕對事件率最高、最不該等」，並給出可在門診使用的量化語言。

## 為什麼重要

門診常見的直覺是「反正相對降幅都差不多，晚一點加沒差」——事實正好相反。finerenone 把心血管複合相對降約 14%、腎臟複合相對降約 23%，這個「打幾折」在不同 eGFR、不同 UACR 幾乎一樣；但同樣打七折，一件一萬元的外套比一件一千元的外套省更多錢。把相對效果的一致性乘上基線事件率的巨大落差，就得到一張可操作的優先順序表。這一頁是 [[次族群分析與效果修飾]] 的臨床輸出面。

## 素材匯總

| 素材 | 對本主題的貢獻 | 證據層級 |
|------|----------------|----------|
| [[2026-07-22-04-04_who_gets_greatest_benefit]] | 「who-benefits-most → who-to-treat-first」的統計橋樑與全套效應量 | 可外推 |
| [[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]] | eGFR×UACR 熱圖 3.7 倍事件率梯度、低 eGFR 的血鉀取捨 | 可外推 |
| [[2026-07-22-04-cluster2_asian_chinese_japanese_subgroup]] | 華人腎臟 NNT 7–12 與其信賴區間 | 可外推 |
| [[2026-07-22-04-cluster3_hf_lvh_targets_insulin_resistance]] | HF 病史、LVH、ADA 目標達標度的 ARR／NNT | 可外推 |
| [[2026-07-22-04-slides_figures_forest_heatmap_nnt]] | RRR vs ARR/NNT 對照總表、簡報校對提醒 | 可外推 |
| [[2026-07-22-04-methodology_subgroup_relative_vs_absolute]] | 「相對一致 → 絕對必異」的定理與 statin 教學數字 | 可外推 |
| [[2026-07-22-04-statistical_insights_myths]] | NNT 的三大內建陷阱，限定本頁所有數字的用法 | 可外推 |
| [[2026-07-22-01-statistical_insights_myths]] | 心衰場景中同一 HR 下 NNT 差 12 倍的平行案例 | 可外推 |

## 核心觀點

1. **地形圖：安慰劑組心血管事件率跨 eGFR×UACR 差 3.7 倍**。每 100 人年，最好一格（eGFR ≥90／UACR <300）為 **2.38（1.03–4.29）**，最差一格（eGFR <30／UACR ≥300）為 **8.74（6.78–10.93）**，單調攀升；而 eGFR×UACR 的交互作用 **P=0.66**。中間各格依序為 ≥90/UACR≥300 3.78（2.91–4.75）；60–<90 為 3.57（2.77–4.48）與 4.76（4.11–5.45）；45–<60 為 4.53（3.72–5.42）與 5.70（4.79–6.70）；30–<45 為 4.93（4.00–5.95）與 6.03（5.14–6.99）；<30/UACR<300 為 6.54（4.19–9.40）（來源：[[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]]、[[2026-07-22-04-slides_figures_forest_heatmap_nnt]]）。

2. **RRR 差 2–3 倍，NNT 差 4–7 倍**。整體 CV NNT **46（29–109）**、整體腎臟 NNT **60（38–142）**（3 年 ARR 1.7%〔0.7–2.6〕）；對照華人腎臟 NNT **7–12**。差距主要來自基線絕對事件率而非療效差異——這就是 who-to-treat-first 的量化語言（來源：[[2026-07-22-04-slides_figures_forest_heatmap_nnt]]）。

3. **華人三份分析的 NNT 一致有利，但 CI 必須一起講**。FIDELITY 中國（N=697）≥57% 腎臟 HR **0.57（0.38–0.86）**、3 年 ARR 8.3%、**NNT 12**；FIGARO 中國（N=325）≥40% 腎臟 HR **0.48（0.29–0.79）**、月 36 **NNT 7（4–22）**；FIDELIO 中國（N=372）≥40% 腎臟 HR **0.59（0.39–0.88）**、30 月 ARR 12.2%、**NNT 8（4–84）**。CI 上界到 22 甚至 84，意思是真值可能要治療 84 人才防一件事（來源：[[2026-07-22-04-cluster2_asian_chinese_japanese_subgroup]]、[[2026-07-22-04-statistical_insights_myths]]）。

4. **有 HF 病史者絕對受益約 3 倍**。效果不被 HF 病史修飾（CV 死亡或首次 HHF 的 **P_interaction=0.81**），但有病史者事件率高得多（54/290＝18.6% vs 無病史 236/3396＝6.7%），48 月 ARR **−4.8%（−13.7 至 4.1）** vs **−1.6%（−3.1 至 0.0）**（來源：[[2026-07-22-04-cluster3_hf_lvh_targets_insulin_resistance]]）。

5. **但沒有 HF 病史也值得用——這是攔截而非治療**。FIGARO 全族群僅 **7.8%（571/7352）** 有 HF 病史，新發 HF **HR 0.68（0.50–0.93）; P=0.016**、48 月 ARR 1.1%、**NNT 91（49–605）**；CV 死亡或首次 HHF HR **0.82（0.70–0.95）**、ARR 1.8%、**NNT 55（29–393）**；首次 HHF HR 0.71（0.56–0.90）、ARR 1.4%、NNT 70（39–292）（來源：[[2026-07-22-04-cluster3_hf_lvh_targets_insulin_resistance]]）。

6. **未達標者絕對事件率最高，達標者仍獲益——所以不應等到危險因子控制達標才加藥**。基線達 0/1/2/≥3 個 ADA 目標者佔 **29%/40%/24%/7%**，安慰劑組 CV 事件率遞減 **6.0 / 5.1 / 4.3 / 3.5** 每 100 人年；但相對效益不因達標而改變（CV P_interaction **0.7481**、腎臟 0.6095、HHF 0.7288、全因死亡 0.0659）（來源：[[2026-07-22-04-cluster3_hf_lvh_targets_insulin_resistance]]）。

7. **個人層級與族群層級要分開講**。NHANES 模擬美國 **640 萬（540–740 萬）** 符合治療者，一年可預防 **38,359 件（31,741–44,852）** 心血管事件，其中 **66%（25,357/38,360）發生於 eGFR ≥60**——因為這群人數龐大。個人層級看事件率排序（低 eGFR／高 UACR 先用）；族群層級看事件總量（eGFR ≥60 的白蛋白尿病人最該常規篩 UACR）（來源：[[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]]）。

8. **層級化取捨：受益最大者血鉀停藥風險也最高**。因高血鉀永久停藥 eGFR <60 為 **2.4% vs 0.8%（安慰劑）**、eGFR ≥60 為 **0.6% vs 0.3%**；高血鉀致住院 eGFR <60 **1.4% vs 0.3%**、eGFR ≥60 **0.3% vs 0%**。這是「用對監測節奏」的理由，不是不用的理由（來源：[[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]]）。

9. **同一個 HR 可以對應 12 倍的 NNT**，在心衰場景亦然：以既有風險模型分五等分，相對效果跨層一致（Q1→Q5 的 HR 為 0.93、1.04、0.82、0.81、0.88，P for interaction = .68），但最低風險 Q1 的絕對下降僅 3.7 per 1000 person-years（**NNT 272**），最高風險 Q5 為 43.0 per 1000 person-years（**NNT 23**）。模型鑑別度好（Q5 vs Q1 事件 HR **10.49**〔8.14–13.52〕）推出的是絕對受益梯度，不是相對療效修飾（來源：[[2026-07-22-01-statistical_insights_myths]]）。

10. **FIDELIO 與 FIGARO 的招募是刻意互補的**，這決定了兩套 NNT 的可移植範圍：FIDELIO 平均 eGFR **44.3**、約 55% eGFR <45、中位 UACR **852**、87.5% UACR ≥300，主要腎臟終點 HR 0.82（0.73–0.93）、3 年 **NNT 29**；FIGARO 平均 eGFR **67.8**、61.7% eGFR ≥60、中位 UACR **308**，CV 複合 HR 0.87（0.76–0.98）、3.5 年 **NNT 47**（來源：[[2026-07-22-04-04_who_gets_greatest_benefit]]）。

11. **操作定義**：以 eGFR × UACR（±HF 病史、±LVH）構成的多維風險估個別病人的基線絕對事件率，再乘上穩定的相對效果（CV 約 14%、腎臟約 23%）得個人化 ARR/NNT。與其逐一問「亞洲人？stage 4？有心衰？」，不如先算這個人的基線風險（來源：[[2026-07-22-04-methodology_subgroup_relative_vs_absolute]]、[[2026-07-22-04-04_who_gets_greatest_benefit]]）。

12. **床邊該有的講法**：「在像您這樣的高風險（高 UACR、低 eGFR）病人、以 3 年為期，大約每 7 到 12 人可避免一次腎臟惡化事件」——時間窗、族群、不確定性一起交代（來源：[[2026-07-22-04-statistical_insights_myths]]）。

## 尚有爭議或未解之處

- **NNT 是綁定時間的**。進階 CKD 亞群腎臟複合終點的 NNT 第 1 年 **41**、第 2 年 **19**、第 3 年 **−40**、第 4 年 **−20**（負值即 NNH，方向翻轉）；同一分析的心血管複合終點 NNT 卻穩定為 1/2/3/4 年 **29/29/31/24**。看到腎臟 NNT 翻負，正確反應不是「後來有害」，而是「這裡本就不該計算單一 NNT」（來源：[[2026-07-22-04-statistical_insights_myths]]）。
- **NNT 不可跨基線風險移植**：整體 NNT 46/60 不能套到高風險華人（7–12），也不能套到低風險早期病人（來源：[[2026-07-22-04-statistical_insights_myths]]）。
- **熱圖事件率是安慰劑組觀察值，不是隨機化對照**；640 萬／38,359 事件為模擬外推；具體數字專屬該試驗族群（中位 UACR 515、平均 eGFR 57.6）（來源：[[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]]）。
- **eGFR <30 這一格的 HR 未被計算**，因比例風險假設不成立；兩組事件率同為約 8.7–8.8 每 100 人年（來源：[[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]]）。
- **「梯度 → hard-outcome 個人化 NNT」的前瞻驗證 RCT 目前不存在**（來源：[[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]]）。
- **死亡率終點的最佳受益族群方向相反**（相對效果在較高基線 eGFR 者更明顯），使「一張優先順序表打天下」不成立（來源：[[2026-07-22-04-04_who_gets_greatest_benefit]]）。

## 關鍵實體

- [[絕對風險差]] — 決定 who-to-treat-first 的真正變量
- [[NNT]] — 綁定時間、族群、且常被省略 CI 的估計值
- [[相對風險與絕對風險]] — 本頁全部推論的量綱基礎
- [[eGFR×UACR 風險分層]] — 熱圖的兩個軸，也是門診最易取得的多維風險
- [[進階 CKD]] — 絕對事件率最高的一格
- [[華人次族群]] — NNT 最小但 CI 最寬的族群
- [[亞洲族群]] — 腎臟事件「底子」較高、故絕對受益放大
- [[心衰竭住院]] — 絕對受益差異最大的終點
- [[左心室肥厚]] — 可能標記 HHF 獲益特別大的一群，屬 hypothesis-generating
- [[基線治療目標達標度]] — 反駁「先控好再加藥」的直接證據
- [[高血鉀]] — 與絕對受益同向增加的代價，須層級化管理
- [[FIDELITY]] — 整體 NNT 與熱圖的資料來源
- [[FIDELIO-DKD]] — 腎臟高風險端的招募
- [[FIGARO-DKD]] — 較早期 CKD／心血管導向的招募
- [[CKD Prognosis Consortium]] — 一般族群風險梯度的外推背景參照
- [[比例風險假設]] — eGFR <30 一格無法給 HR 的原因

## 相關頁面

- [[次族群分析與效果修飾]]
- [[臨床統計素養與常見陷阱]]
- [[高血鉀安全工程]]
- [[效益風險權衡與指引仿單框架]]
