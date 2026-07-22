---
tags: [素材摘要, 簡報數據, 熱圖, 森林圖, NNT]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/04-slides_figures_forest_heatmap_nnt.md
images: 0
image_paths: []
---

# 建議圖表 · 簡報數據總表：熱圖、森林圖、RRR/ARR/NNT

> 四張圖把「相對一致 → 絕對受益隨基線風險放大 → who-to-treat-first」的視覺骨架講完，並附上台前必須二次核對的載重數字清單。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/04-slides_figures_forest_heatmap_nnt.md
- **消化日期**：2026-07-22

## 核心觀點

1. **圖 1 熱圖 — eGFR×UACR 的絕對事件率**（FIDELITY 安慰劑組，每 100 人年，Agarwal 2023）📄🟡。左上（eGFR ≥90／UACR <300）**2.38（1.03–4.29）** → 右下（eGFR <30／UACR ≥300）**8.74（6.78–10.93）**，單調攀升約 **3.7 倍**。中間各格：≥90/UACR≥300 3.78（2.91–4.75）；60–<90 3.57（2.77–4.48）與 4.76（4.11–5.45）；45–<60 4.53（3.72–5.42）與 5.70（4.79–6.70）；30–<45 4.93（4.00–5.95）與 6.03（5.14–6.99）；<30/UACR<300 6.54（4.19–9.40）。**顏色概念**：數字愈大＝絕對事件率愈高＝同一相對效果下 NNT 愈小＝愈值得早用。

2. **熱圖的外推背景參照**📄。CKD Prognosis Consortium（Matsushita 2010）顯示一般族群 eGFR 60/45/15（vs 95）全因死亡校正 HR **1.18/1.57/3.14**；UACR 10/30/300（vs 5）HR **1.20/1.63/2.22**，且 eGFR 與 UACR **相乘、無交互**——與試驗內的絕對事件率梯度同向，支持熱圖的外推性。

3. **圖 2 森林圖 — 各面向次族群的相對效果**🟡。eGFR×UACR 全譜／複合 CV HR 0.86（0.78–0.95），P_int 0.66；各 eGFR 分層／≥57% 腎臟 0.77（0.67–0.88），P_int 0.62；亞洲 vs 非亞洲／≥57% 腎臟 0.64（0.50–0.82），P_int 0.0493；／≥40% 腎臟 0.67（0.56–0.80），P_int 0.0009；／複合 CV 0.90（0.70–1.15），P_int 0.8454；華人（FIDELITY）／≥57% 腎臟 0.57（0.38–0.86），P_int 0.15；有無 HF 病史／CV 死亡或首次 HHF 0.82（0.70–0.95），NS；LVH vs 無 LVH／HHF **0.34（0.19–0.61）**，**P_int 0.0024**；達 0/1/2/≥3 目標／複合 CV 0.86（整體），P_int 0.7481📄。

4. **讀圖要點**：除 LVH×HHF 外交互作用多不顯著——**點估計的散布主要反映各亞群的事件數／樣本量，而非真實效果修飾**。相對效果的「一致」正是絕對受益梯度的前提。LVH×HHF 雖顯著，但屬事後、ECG 無中央裁決、未校正多重性 → 標為 hypothesis-generating【尚待驗證】。

5. **圖 3 表 — RRR 與 ARR/NNT 分開呈現**🟡。FIDELITY 整體 CV 14%（0.86），NNT **46（29–109）**；FIDELITY 整體腎臟 23%（0.77），3 年 ARR 1.7%（0.7–2.6），NNT **60（38–142）**；FIDELIO 整體主要腎臟 18%（0.82），NNT **29**（3 年）；FIGARO 新發 HF 32%（0.68），48 月 ARR 1.1%，NNT **91（49–605）**；FIGARO CV 死亡或首次 HHF 18%（0.82），ARR 1.8%，NNT **55（29–393）**；FIGARO 首次 HHF 29%（0.71），ARR 1.4%，NNT **70（39–292）**；華人 FIDELITY ≥57% 腎臟 43%（0.57），3 年 ARR 8.3%，**NNT 12**；華人 FIGARO ≥40% 腎臟 52%（0.48），**NNT 7（4–22）**；華人 FIDELIO ≥40% 腎臟 41%（0.59），30 月 ARR 12.2%，**NNT 8（4–84）**📄。

6. **圖 3 的核心對照**：整體 CV NNT 46 vs 華人腎臟 NNT 7–12——**RRR 差異只有 2–3 倍，但 NNT 差異達 4–7 倍**，差距主要來自基線絕對事件率（華人高 UACR、腎臟事件率高）。這就是 who-to-treat-first 的量化語言。注意華人 NNT 的 CI 寬（如 Zhang 4–84），反映小樣本不確定性🔴。

7. **圖 4 Mermaid 流程**：平均治療效果（FIDELITY CV HR 0.86／腎臟 HR 0.77）→ 相對效果是否跨次族群一致？→ 是（多數 P_interaction 不顯著）則「相對一致 ≠ 人人同樣受益」（Sun 2010／Yusuf 1991）；少數顯著（如 LVH×HHF P=0.0024）則標為 hypothesis-generating 待外部重現（Wallach 2017／ICEMAN）→ 以多維基線風險估算絕對事件率 → 絕對事件率愈高則 ARR 愈大、NNT 愈小 → 精準層級判讀 who-to-treat-first → 同時層級化血鉀風險 → 門診 individualized layering。

8. **8–10 分鐘的講法建議**：開場用熱圖建立「3.7 倍地形」直覺；承接用森林圖強調「一致 ≠ 一樣受益」；核心用「RRR 差 2–3 倍、NNT 差 4–7 倍」一句話把絕對受益放大講死；收束用流程圖帶到血鉀層級化取捨（銜接主題五）。

9. **⚠ 簡報校對提醒（載重數字上台前二次核對）**：(a) 圖 2 的「各 eGFR 分層 ≥57% 腎臟 HR 0.77」及其分層 HR，來源 `stage4_ckd_Bakris_2023.md` 表格於 PDF→Markdown 轉檔時有**欄位上移**情形，分層 HR（尤其 eGFR ≥60）建議回原始 Kidney International Table 1 核對；(b) 華人 NNT（7／8／12）小樣本、CI 寬，務必連同 CI 呈現，避免給人「華人一定 NNT<10」的過度印象；(c) LVH×HHF HR 0.34 為唯一顯著交互但屬事後探索，投影片應標 hypothesis-generating。

## 關鍵概念

[[Finerenone]]、[[FIDELITY]]、[[NNT]]、[[絕對風險差]]、[[交互作用檢定]]、[[eGFR×UACR 風險分層]]、[[左心室肥厚]]、[[華人次族群]]、[[CKD Prognosis Consortium]]

## 與其他素材的關聯

- 本檔為 [[2026-07-22-04-04_who_gets_greatest_benefit]] §7 的獨立簡報數據總表，數字全部來自四個延伸檔。
- 圖 1 熱圖與 Bakris 表格校正註源自 [[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]]。
- 圖 2、圖 3 的亞洲／華人列源自 [[2026-07-22-04-cluster2_asian_chinese_japanese_subgroup]]；LVH 與 HF 列源自 [[2026-07-22-04-cluster3_hf_lvh_targets_insulin_resistance]]。
- 圖 4 的方法學節點（Sun 2010／Yusuf 1991／Wallach 2017／ICEMAN）詳見 [[2026-07-22-04-methodology_subgroup_relative_vs_absolute]]。
- 「NNT 必須連 CI 一起講」的告誡在 [[2026-07-22-04-statistical_insights_myths]] 迷思一被展開為 NNT 的三大內建陷阱。
- 此檔是唯一同時列出全部圖表數據的檔案，最適合作為投影片製作的單一入口。<!-- confidence: INFERRED -->

## 原文精彩摘錄

> **讀圖**：左上（腎功能好、低白蛋白尿）到右下（低 eGFR、高 UACR），事件率單調攀升約 **3.7 倍**（2.38 → 8.74）。同樣的相對效果，套在右下角的人身上省下的絕對事件最多。

> **對照**第一列（整體 CV NNT 46）與末三列（華人腎臟 NNT 7–12）：**RRR 差異只有 2–3 倍，但 NNT 差異達 4–7 倍**，差距主要來自基線絕對事件率。

> **華人 NNT（7 / 8 / 12）**：小樣本、CI 寬，簡報時務必連同 CI 呈現，避免給人「華人一定 NNT<10」的過度印象。

## 相關頁面
