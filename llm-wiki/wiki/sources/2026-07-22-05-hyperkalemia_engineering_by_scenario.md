---
tags: [素材摘要, 高血鉀, 風險修飾因子, 安全性監測, IPD pooled]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/05-hyperkalemia_engineering_by_scenario.md
images: 0
image_paths: []
---

# 高血鉀的工程學：按場景、研究設計與風險修飾因子拆開

> finerenone 的高血鉀「風險」不是單一數字，而是隨研究型態、eGFR、baseline K⁺、併用藥而變的一組數字——拆開之後「相對約 2 倍、絕對硬結局低」才從口號變成可操作的門診決策。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/05-hyperkalemia_engineering_by_scenario.md
- **消化日期**：2026-07-22

## 核心觀點

1. **同一顆藥、八種切法、八組數字**：整體 pooled 約 14%、進階 CKD 單試驗約 21%、Stage 4 亞群約 26%、心衰場景反而約 10%、合併 SGLT2i 不放大甚至略降。原文明確警告：**這些列不能直接互比絕對數字**，因分母、事件定義（investigator-reported vs 中央實驗室 K⁺ 閾值）、追蹤長度、族群風險都不同；共同不變量只有方向與量級 📄。

2. **FIDELIO-DKD（中位追蹤 2.6 年）把風險量化得最完整**：≥mild 高血鉀 **597/2785（21.4%）vs 256/2775（9.2%）**、≥moderate(>6.0) **126/2802（4.5%）vs 38/2796（1.4%）**。處置以暫時撤藥為主——藥物**中斷** 310（11.0%）vs 146（5.2%）、**撤除** 64（2.3%）vs 25（0.9%）；多變量校正後獨立 **HR 2.13（1.86–2.45），P<0.0001** 📄（post hoc）。

3. **Stage 4 亞群（n=890，7%；平均 eGFR 26.9、中位 UACR 720 mg/g）**：高血鉀 **26% vs 13%**（翻倍），但永久停藥僅 **3% vs 2%**、住院 3% vs 1%、**無高血鉀死亡**。血鉀變化溫和——月 4 平均變化 **0.26（SD 0.51）vs 0.02（SD 0.49）**。同時保有心腎益處：CV composite **HR 0.78（0.57–1.07）**、chronic eGFR slope 由 **−3.2 改善至 −1.8 mL/min/年（差 1.39；0.48–2.30；P=0.04）**、UACR 月 4 降 31% 📄（亞群 post hoc；kidney composite 之比例風險假設 2 年後不成立，作者標為 exploratory）。

4. **心衰場景（FINEARTS-HF）高血鉀反而較輕**：9.7% vs 4.2%、永久停藥 0.4% vs 0.2%。Vardeny 次分析：K⁺ >5.5 **HR 2.16（1.83–2.56）**、>6.0 **HR 2.07（1.4–3.0）**、K⁺ <3.5 **HR 0.46（0.38–0.56）**；跨劑量一致（20-mg 層 HR 2.02、40-mg 層 HR 2.35，interaction P=.39）。**關鍵**：即使第 1 個月即升至 >5.5，療效仍維持——經歷 vs 未經歷 K⁺ >5.5 之 **HR 0.84（0.55–1.30）vs 0.83（0.74–0.92），interaction P=.72** 📄。

5. **兩份 2026 prespecified IPD pooled**：**INFINITY**（n=14,574，首度納入非糖尿病 CKD／FIND-CKD）任一高血鉀 **14.3%（1043）vs 7.6%（553）**、永久停藥 1.7%（122）vs 0.5%（39）、serious 1.1% vs 0.3%、住院 0.9% vs 0.2%、**fatal 0 vs 0**；實驗室 K>5.5 **17.0% vs 7.9%**、K<3.5 3.6% vs 8.0%。**FINE-HEART**（n=14,180）實驗室 K>5.5 **18% vs 8%**、K>6.0 4%、永久停藥 2% vs 1%、住院 1%（69）vs 0.2%（15）、無高血鉀死亡；SAE 反而 finerenone 較低（34% vs 36%）；每處方約 **131** 人才 1 次高血鉀相關住院，同一分析 CV death/HHF **HR 0.83（0.75–0.93）、NNT 60** 📄。

6. **「相對約 2 倍」在三種完全不同設計下高度一致**：7-study 統合 RR **2.09**、FIDELIO 單試驗多變量 HR **2.13**、FINEARTS-HF 次分析 HR **2.16**。差異全落在「絕對事件」層——住院 <1%–3%、永久停藥 0.4%–3%、死亡 0，因為**協議化監測＋暫停/減量把重症攔截掉了** 📄。

7. **KDIGO 2026 草案 7-study 統合（7 studies、41 reports、nsMRA[finerenone 或 esaxerenone] vs placebo、全數排除 eGFR<25）**：hyperkalemia RR **2.09（1.82–2.39）**、K ≥5.5 RR **2.18（1.98–2.40）**；療效端 kidney composite **HR 0.84（0.77–0.92）**、kidney failure **HR 0.84（0.71–0.99）**、HF/HHF **HR 0.78（0.66–0.92）**顯著，而 all-cause mortality RR 0.90（0.81–1.00）、CV mortality RR 0.88（0.76–1.02）、stroke RR 1.01、nonfatal MI RR 0.92 未達顯著；kidney failure／HHF／kidney composite 三項證據確定性為 **high** 📄（**尚待驗證：公開審查草案、尚未定稿**）。

8. **風險修飾因子表（本檔最重要的「工程學」）**——FIDELIO 多變量 Cox 對 ≥mild 高血鉀之獨立預測因子：baseline K⁺ >5.0 **HR 4.18（3.45–5.05）**、4.8–5.0 **2.78**、4.5–4.8 **1.53**、≤4.1 **0.44（低起點保護）**；eGFR <25 **2.04（1.35–3.07）**、25–<45 **1.51**、45–<60 **1.02**；每倍 UACR（log2）**1.12**；β-blocker **1.18（1.04–1.35）**；利尿劑 **0.76（0.66–0.87）**；**SGLT2i 0.45（0.27–0.75）**；ACEi/ARB 劑量不顯著（P=0.8508）📄。

9. **eGFR 分層的絕對事件（Bakris FIDELITY）**：任一 investigator-reported 高血鉀 eGFR<60 **714（18.3%）vs 333（8.5%）**、eGFR≥60 **198（7.6%）vs 115（4.4%）**；因高血鉀永久停藥 eGFR<60 **2.4% vs 0.8%**、eGFR≥60 0.6% vs 0.3%；住院 eGFR<60 1.4% vs 0.3%、eGFR≥60 0.3% vs 0%。結論：**低 eGFR 是「監測更勤」的訊號，不是禁忌** 📄。

10. **併用 SGLT2i／GLP-1RA 未放大高血鉀，但不可倚賴其「抵銷」**：CONFIDENCE very-high risk 亞群實驗室 K⁺ >5.5 combo **19.6%** vs finerenone **22.3%** vs empagliflozin 10.3%；GLP-1RA 次分析（n=800，182[23%] 用 GLP-1RA）combo 高血鉀率 **9.0% vs 9.5%** 幾乎相同；FIDELITY 次分析明言安全輪廓不因併用而改變。**誠實邊界**：KDIGO 2026 草案明白寫道「the addition of empagliflozin to finerenone did not appear to mitigate the effect of hyperkalemia with an nsMRA」——**不放大 ≠ 消除，監測不可省** 📄。

11. **血鉀「可回收」的三個動力學事實**：(a) 幅度小且平台化——組間平均差最大僅 **0.23 mmol/L（月 4）**，EMA 記載首月 ≤0.2 mmol/L 後穩定；(b) 短半衰期 **2–3 小時**、無活性代謝物，故 K⁺ >5.5 暫停、≤5.0 以 10 mg 重啟；(c) FIDELIO spline 顯示月 4 時同樣 0.5 mmol/L 上升，**安慰劑對應約 3.4 倍**後續高血鉀風險而 **finerenone 僅約 2 倍**（組間差異 P=0.011）📄。

## 關鍵概念

- [[高血鉀]]
- [[血鉀監測]]
- [[Finerenone]]
- [[Empagliflozin]]
- [[FIDELIO-DKD]]
- [[FIDELITY]]
- [[FINEARTS-HF]]
- [[INFINITY]]
- [[FINE-HEART]]
- [[CONFIDENCE]]
- [[KDIGO 2026 糖尿病與 CKD 指引草案]]

## 與其他素材的關聯

本檔是主題五主文 §3「表 5」的展開版，把一張並列表拆成三個維度（場景／研究設計／修飾因子）。與 [[2026-07-22-05-05_hyperkalemia_egfr_dip_safety_engineering]] 共用 FIDELIO HR 2.13、Stage 4 26% vs 13%、SGLT2i HR 0.45 等錨點數字，但本檔額外補上 Bakris eGFR 分層絕對事件與 INFINITY／FINE-HEART 的完整分子分母。

風險修飾因子表直接餵給 [[2026-07-22-05-outpatient_workflow_monitoring_algorithm]] 的「起始前檢核」與「加密監測觸發清單」；「暫停即可回收」的半衰期論證則同時支撐 workflow 檔的暫停-重啟規則與 [[2026-07-22-05-cyp3a4_interaction_prescribing_rules]] 的「暫停即解毒」安全網。
<!-- confidence: INFERRED --> 原文自陳「無 binder-enabled finerenone 硬終點 RCT」並指向 `potassium_binder_role.md`，兩檔在「反覆 >5.5 該停藥還是加 binder」的分岔點上互補。

## 原文精彩摘錄

> 「這六（八）列**不能直接互比絕對數字**，因為分母、事件定義（investigator-reported vs 中央實驗室 K⁺ 閾值）、追蹤長度、族群風險都不同。它們的**共同不變量**是方向與量級——相對約 2 倍、絕對硬結局低、幾乎零高血鉀死亡。」

> 「這張表就是『選對病人＋調對背景藥』的清單——**baseline K⁺ 與 eGFR 是最大槓桿**（起始前把 K⁺ 控在 ≤5.0、eGFR ≥25）；**SGLT2i 與利尿劑是內建的降鉀夥伴**；β-blocker 是隱形的升鉀因子（不是禁忌，是監測訊號）。」

> 「正確的門診話術是：**併用 SGLT2i「不放大、甚至數值略降」高血鉀，但不能倚賴它「抵銷」——監測仍不可省**。」

## 相關頁面

- [[2026-07-22-05-05_hyperkalemia_egfr_dip_safety_engineering]]
- [[2026-07-22-05-outpatient_workflow_monitoring_algorithm]]
- [[2026-07-22-05-potassium_binder_role]]
- [[2026-07-22-05-egfr_dip_hemodynamic_reversible]]
