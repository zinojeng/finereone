---
tags: [素材摘要, 進階 CKD, 絕對風險, 高血鉀, 死亡率]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/04-cluster1_advanced_ckd_absolute_event_gradient.md
images: 0
image_paths: []
---

# 叢集一 · 進階 CKD 與 eGFR×UACR 的絕對事件率梯度

> 相對療效在整個 eGFR×UACR 譜上一致，正因為一致，腎功能最差、白蛋白尿最重的病人才是 ARR 最大、NNT 最小、最不該等的一群。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/04-cluster1_advanced_ckd_absolute_event_gradient.md
- **消化日期**：2026-07-22

## 核心觀點

1. **門診常見的直覺講反了**。「反正相對降幅都差不多，晚一點加沒差」——事實相反。finerenone 把心血管複合相對降約 14%、腎臟複合相對降約 23%，這個「打幾折」在不同 eGFR/UACR 幾乎一樣；但同樣打七折，一件一萬元外套比一件一千元外套省更多錢。本檔只建立在四份本地全文之上（Agarwal 2023、Bakris 2023、Filippatos 2023、Sun 2010），全部 📄；abstract-only 的 Zhao 2026／Zuin 2026 不屬本叢集。

2. **方法學地基（Sun 2010）**🟡。原文為「if no subgroup effect is associated with these factors for relative measures of effect, a subgroup effect for absolute measures must exist」📄。statin 範例：相對降 **29.2%** 一致，10 年風險 5% 者只換得 **ARR 1.5%（5%→3.5%）**，10 年風險 50% 者換得 **ARR 14.6%（50%→35.4%）**——同一相對效果，絕對受益差近 10 倍。所以次分析裡「一堆不顯著的交互作用 P 值」不是「人人受益一樣」的證據，而是「絕對受益梯度存在」的保證書。

3. **熱圖梯度（Agarwal 2023，JAMA Cardiol）**🟡。安慰劑組每 100 人年複合心血管事件率（CV death、非致死中風、非致死 MI、HF 住院）：最好一格 eGFR ≥90／UACR <300 為 **2.38（1.03–4.29）**，最差一格 eGFR <30／UACR ≥300 為 **8.74（6.78–10.93）**，約 **3.7 倍**📄。整體療效 **HR 0.86（0.78–0.95），P=.002**；eGFR×UACR **交互作用 P=.66**。

4. **兩個尺度必須分開講**。NHANES 模擬美國 **640 萬（95% CI 540–740 萬）** 符合治療者，一年預防 **38,359 件（31,741–44,852）** 心血管事件，其中 **66%（25,357/38,360）發生於 eGFR ≥60**📄。這不與「低 eGFR 個別風險最高」矛盾——**個人層級**看絕對事件率排序（低 eGFR/高 UACR 先用）；**族群／公衛層級**看事件總量（eGFR ≥60 的白蛋白尿病人最該常規篩 UACR）。

5. **腎臟終點（Bakris 2023，Kidney Int，prespecified exploratory）**🟡。整體腎臟複合 finerenone **360/6519（5.5%）** vs placebo **465/6507（7.1%）**，HR **0.77（0.67–0.88），P=0.0002**，3 年絕對組間差 **1.7%（0.7–2.6）**，**NNT 60（38–142）**📄。ESKD HR 0.80（0.64–0.99，P=0.040）；持續 ≥57% eGFR 下降 HR 0.70（0.60–0.83，P<0.0001）。分層 P_interaction：eGFR 0.62、UACR 0.67，方向一致；但 **UACR 30–<300 亞群 HR 0.94（0.60–1.47）** 不確定性高——「一致 ≠ 每一格都精確」。

6. **森林圖細節（Bakris Figure 3，by 基線 eGFR）**：eGFR <30 事件率 finerenone 8.80 vs placebo 8.73 每 100PY，**HR 因 Cox 比例風險假設不成立而未計算**——但兩組事件率同為 ~8.7–8.8，凸顯此族群絕對事件率最高；30–<60 HR 0.72（0.59–0.88）；60–<90 HR 0.78（0.57–1.05）；≥90 HR 0.44（0.22–0.86）📄。⚠️ 原稿標註 `stage4_ckd_Bakris_2023.md` 行 199–206 表格於 PDF→Markdown 轉檔時**欄位上移一列**，eGFR ≥60 列真正的 HR 為 0.70（0.53–0.92）而非該位置顯示的 1.66（1.38–1.95，實為每 100 人年事件率）；判定依據為事件數 90/2603（3.5%）vs 130/2592（5.0%），HR 必 <1。做簡報前建議回原始 Kidney International Table 1 二次核對。

7. **低 eGFR 的血鉀取捨**（Bakris Table 2）：因高血鉀停藥 eGFR <60 **2.4% vs 0.8%（placebo）**、eGFR ≥60 **0.6% vs 0.3%**；高血鉀致住院 eGFR <60 **1.4% vs 0.3%**、eGFR ≥60 **0.3% vs 0%**；中央實驗室 K⁺ >5.5：eGFR <60 20.5% vs 8.7%、eGFR ≥60 11.2% vs 5.4%；K⁺ >6.0：4.2% vs 1.3% 與 1.9% vs 1.2%📄。**最該被保住治療的低 eGFR 病人，也最容易因血鉀而停藥**——這是要「用對監測節奏」的理由，不是不用的理由。

8. **死亡率的反向梯度（Filippatos 2023，EHJ-CVP）**🟡。全因死亡 ITT 8.5% vs 9.4%，HR 0.89（0.79–1.00，P=0.051）；on-treatment 4.3% vs 5.3%，HR 0.82（0.70–0.96，P=0.014）。CV 死亡 ITT 4.9% vs 5.6%，HR 0.88（0.76–1.02，P=0.092）；on-treatment 2.9% vs 3.6%，HR 0.82（0.67–0.99，P=0.040）。猝死 ITT 1.3%（0.44/100PY）vs 1.8%（0.58/100PY），HR 0.75（0.57–0.996，P=0.046）📄。KDIGO 風險組人數：low 64、moderate 1,323、high 5,345、very high 6,288。無 KDIGO 交互（全因 P-int 0.1293、CV 0.6361），但效果「more pronounced in patients with higher baseline eGFR」。**尚待驗證**：死亡率顯著性依賴 on-treatment 分析與猝死次要終點，不宜講成「已證實降低死亡率」🔴。

9. **誠實邊界**：三份 FIDELITY 次分析 P 值均未校正多重比較；熱圖事件率為安慰劑組觀察值而非隨機化對照；NHANES 640 萬／38,359 事件為模擬外推；具體數字專屬 FIDELITY 族群（median UACR 515、mean eGFR 57.6）；「梯度 → hard-outcome 個人化 NNT」之前瞻驗證 RCT **目前不存在**🔴。

## 關鍵概念

[[Finerenone]]、[[FIDELITY]]、[[進階 CKD]]、[[絕對風險差]]、[[NNT]]、[[交互作用檢定]]、[[高血鉀]]、[[eGFR×UACR 風險分層]]、[[比例風險假設]]、[[交互作用檢定]]

## 與其他素材的關聯

- 本檔為 [[2026-07-22-04-04_who_gets_greatest_benefit]] §3 的延伸拆解。
- 方法學地基（Sun 2010）與 [[2026-07-22-04-methodology_subgroup_relative_vs_absolute]] 共用同一組 statin 教學數字。
- 熱圖與森林圖數據被 [[2026-07-22-04-slides_figures_forest_heatmap_nnt]] 收錄為圖 1、圖 2。
- Bakris 表格欄位上移的校正註同時出現在簡報總表的「校對提醒」。<!-- confidence: EXTRACTED -->
- eGFR <30 亞群 HR 未計算（PH 假設不成立）與 [[2026-07-22-04-statistical_insights_myths]] 迷思四（PH 失效）直接呼應。<!-- confidence: INFERRED -->
- 低 eGFR 血鉀停藥率銜接主題五之高血鉀監測 workflow。<!-- confidence: INFERRED -->

## 原文精彩摘錄

> 用最白話的方式說：finerenone 大概把心血管複合事件相對降 **14%**、腎臟複合事件相對降 **23%**，而且這個「打幾折」在不同 eGFR、不同 UACR 的病人身上幾乎一樣。但「打一樣的折」套在「本來風險就高的人」身上，省下來的**絕對數字**就大得多——就像同樣打七折，一件一萬元的外套比一件一千元的外套省更多錢。

> 也就是說，**最該被保住治療的低 eGFR 病人，同時也是最容易因血鉀而停藥的病人**——這不是理由不用，而是理由要「用對監測節奏」。

> 關鍵洞見是——**不同終點的「最佳受益族群」可以不同**：腎臟/HF 終點的絕對受益在低 eGFR 者最大，死亡率終點的相對效果在高 eGFR 者更明顯。

## 相關頁面
