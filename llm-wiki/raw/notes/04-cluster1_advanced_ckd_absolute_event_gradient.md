# 叢集一 · 進階 CKD 與 eGFR×UACR 的絕對事件率梯度：who-to-treat-first 的核心證據

> 本檔為主題四（誰得到最大效益）§3「叢集一」之**延伸拆解＋簡報數據集**。核心命題只有一句、但值得反覆講：finerenone 的**相對療效**在 eGFR×UACR 的整個譜上大致一致，正因為一致，**絕對受益必隨基線事件率放大**——所以「腎功能最差、白蛋白尿最重」的病人，雖然相對風險降幅一樣，卻是 ARR 最大、NNT 最小、最值得「現在就用、不要等」的一群。這就是把「who-benefits-most」翻成「who-to-treat-first」的統計橋樑。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（不對其未載內容作具體數字斷言）。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織與改寫，所有作者／年份／數字均出自本地 MD 檔。
>
> **證據分層**：🟢 guideline routine（已進指引常規）｜🟡 evidence expansion（prespecified／exploratory／post hoc／次分析／代理終點）｜🔴 尚待驗證（無直接 hard-outcome RCT，或屬未定稿草案）。
>
> **本檔誠實立場**：本叢集**只**建立在四份本地全文之上（Agarwal 2023、Bakris 2023、Filippatos 2023、Sun 2010），全部 📄。abstract-only 的 Zhao 2026／Zuin 2026 不屬本叢集、其數字不在此擴張。

---

## 0. 門診一句話：為什麼「相對一樣」反而是「早用」的理由

門診常見的直覺是：「反正相對降幅都差不多，那晚一點加 finerenone 也沒差。」這句話**恰好講反了**。

用最白話的方式說：finerenone 大概把心血管複合事件相對降 **14%**、腎臟複合事件相對降 **23%**，而且這個「打幾折」在不同 eGFR、不同 UACR 的病人身上幾乎一樣 [stage4_ckd_Agarwal_2022] 📄。但「打一樣的折」套在「本來風險就高的人」身上，省下來的**絕對數字**就大得多——就像同樣打七折，一件一萬元的外套比一件一千元的外套省更多錢。所以腎功能差、白蛋白尿高的病人，才是「早一點用、每治療較少人就能避免一個事件」的族群。這是本檔所有數字要證明的一件事。

---

## 1. 方法學地基：一致的相對效果「必然」製造絕對受益的差異（Sun 2010）🟡

先把統計橋樑釘牢，後面的臨床數字才站得住。

Sun 2010（BMJ，subgroup 可信度準則）給了決定性的一句話：在已知預後因子能把病人分成不同風險組的前提下，**若相對效果對這些因子沒有交互作用，則絕對效果的 subgroup effect 就「必然存在」**——原文為「if no subgroup effect is associated with these factors for relative measures of effect, a subgroup effect for absolute measures must exist」[subgroup_methodology_Sun_2010] 📄。

作者的 statin 教科書範例把這件事量化得很乾淨：statin 對主要冠狀動脈事件的**相對**降幅 **29.2%** 跨次族群一致，但套到 10 年風險 5% 的低危病人只換得 **ARR 1.5%（5%→3.5%）**，套到 10 年風險 50% 的高危病人卻換得 **ARR 14.6%（50%→35.4%）**[subgroup_methodology_Sun_2010] 📄。同一個相對效果，絕對受益差了將近 10 倍——差別完全來自基線風險。

> **臨床轉譯**：所以當我們在 finerenone 的次分析裡看到「一堆不顯著的交互作用 P 值」，那**不是**「人人受益一樣」的證據，而是「絕對受益梯度存在」的**保證書**。把這句話記牢，下一節的熱圖就會自己說話。

---

## 2. 絕對事件率梯度：eGFR 越低、UACR 越高，安慰劑組事件率單調攀升（Agarwal 2023）🟡

Agarwal 2023（JAMA Cardiology，FIDELITY「可修飾性」次分析）提供了本主題**最關鍵的一張熱圖**：把 13,026 名病人按基線 eGFR×UACR 切格，看**安慰劑組**每 100 人年的複合心血管事件率（心血管death、非致死中風、非致死 MI、HF 住院）[stage4_ckd_Agarwal_2023] 📄。

- 最好的一格（eGFR ≥90 且 UACR <300）：**2.38（95% CI 1.03–4.29）**每 100 人年 [stage4_ckd_Agarwal_2023] 📄。
- 最差的一格（eGFR <30 且 UACR ≥300）：**8.74（95% CI 6.78–10.93）**每 100 人年 [stage4_ckd_Agarwal_2023] 📄。
- 兩端相差約 **3.7 倍**——這就是「基線絕對風險」的地形圖。

而 finerenone 的相對效果對這個梯度**幾乎不敏感**：整體 **HR 0.86（95% CI 0.78–0.95；P = .002）**，eGFR×UACR 的**交互作用 P = .66**[stage4_ckd_Agarwal_2023] 📄。這正是第 1 節 Sun 2010 所述「相對恆定、絕對放大」的教科書範例。

**一個容易講錯、必須分兩個尺度講的反直覺點**：Agarwal 2023 以 NHANES 模擬美國約 **6.4 百萬（95% CI 5.4–7.4 million）**符合治療條件者，估計一年治療可預防 **38,359 件（95% CI 31,741–44,852）**心血管事件，其中 **66%（25,357 of 38,360）發生在 eGFR ≥60 的病人**[stage4_ckd_Agarwal_2023] 📄。這**不**與「低 eGFR 者個別絕對風險最高」矛盾——因為 eGFR ≥60 但有白蛋白尿的病人**人數龐大**：個別絕對風險不是最高，但族群層級的可預防事件**總量**最大。

> **講者必須清楚區分兩個尺度**：**個人層級**看絕對事件率排序（低 eGFR/高 UACR 先用）；**族群/公衛層級**看事件總量（eGFR ≥60 的白蛋白尿病人是被低估、最該常規做 UACR 篩檢的一群）[stage4_ckd_Agarwal_2023] 📄。兩者都對，只是問的問題不同。

---

## 3. 進階/低 eGFR 的腎臟終點：相對效果維持，但不確定性與血鉀同時放大（Bakris 2023）🟡

Bakris 2023（Kidney International，FIDELITY 腎臟 prespecified exploratory 分析）把「腎臟終點」這一面講透 [stage4_ckd_Bakris_2023] 📄。

**整體腎臟複合終點**（kidney failure、持續 ≥57% eGFR 下降、腎death）：finerenone **360/6519（5.5%）** vs placebo **465/6507（7.1%）**，相對降 **23%（HR 0.77；95% CI 0.67–0.88；P = 0.0002）**，3 年**絕對組間差 1.7%（95% CI 0.7–2.6）**，**NNT 60（95% CI 38–142）**[stage4_ckd_Bakris_2023] 📄。ESKD 相對降 **20%（HR 0.80；95% CI 0.64–0.99；P = 0.040）**；持續 ≥57% eGFR 下降這一分項降 **30%（HR 0.70；95% CI 0.60–0.83；P < 0.0001）**[stage4_ckd_Bakris_2023] 📄。

**跨基線 eGFR/UACR 分層方向一致、但要誠實標示不確定性**：eGFR 分層 **Pinteraction = 0.62**、UACR 分層 **Pinteraction = 0.67**，方向一致；但作者明言 **UACR 30–<300 mg/g 亞群不確定性高**（HR 0.94；95% CI 0.60–1.47，CI 很寬）[stage4_ckd_Bakris_2023] 📄。這就是「一致 ≠ 每一格都精確」的活教材——白蛋白尿較輕的人，事件少、CI 寬，點估計不能過度解讀。

**低 eGFR 的「層級化取捨」——受益最大、血鉀代價也最大**：這是門診最實用的一句。血鉀導致停藥在 **eGFR <60 為 2.4%（finerenone）vs 0.8%（placebo）**，在 **eGFR ≥60 僅 0.6% vs 0.3%**；血鉀住院在 eGFR <60 為 **1.4% vs 0.3%**、eGFR ≥60 為 **0.3% vs 0%**[stage4_ckd_Bakris_2023] 📄。也就是說，**最該被保住治療的低 eGFR 病人，同時也是最容易因血鉀而停藥的病人**——這不是理由不用，而是理由要「用對監測節奏」（見主題五 eGFR dip 與高血鉀工程學檔）。

作者的收尾與本檔命題完全同調：finerenone「provides robust kidney efficacy and safety benefits across the spectrum of CKD in T2D and highlights the benefits of early treatment initiation to slow CKD progression」[stage4_ckd_Bakris_2023] 📄。

---

## 4. 死亡率的「反向梯度」：不同終點的最佳受益族群可以不同（Filippatos 2023）🟡

這一節最容易被講成矛盾，其實是本主題最漂亮的深度點。

Filippatos 2023（EHJ-CVP，FIDELITY 死亡率分析）發現：全因死亡 **ITT HR 0.89（95% CI 0.79–1.00；P = 0.051）**、CV 死亡 **ITT HR 0.88（95% CI 0.76–1.02；P = 0.092）**都是**邊緣不顯著**；但 **on-treatment** 分析都顯著——全因 **HR 0.82（0.70–0.96；P = 0.014）**、CV **HR 0.82（0.67–0.99；P = 0.040）**；猝死 ITT 亦顯著下降 **HR 0.75（0.57–0.996；P = 0.046）**[stage4_ckd_Filippatos_2023] 📄。

死亡率效果**跨 KDIGO 風險組一致**（全因 **Pinteraction = 0.1293**、CV **Pinteraction = 0.6361**），但作者觀察到「seemingly more pronounced in patients with higher baseline eGFR」——**死亡率這個特定終點，反而在較高基線 eGFR 者更明顯**[stage4_ckd_Filippatos_2023] 📄。

> **對讀重點（易誤講）**：這與「低 eGFR 者腎臟/心血管絕對事件率最高」**並不衝突**。作者的解讀是：低 eGFR 病人器官損傷已重、較難逆轉，故**死亡率**這個終點的相對效果在早期（高 eGFR）更強，暗示「早用可爭取更多存活效益」[stage4_ckd_Filippatos_2023] 📄。關鍵洞見是——**不同終點的「最佳受益族群」可以不同**：腎臟/HF 終點的絕對受益在低 eGFR 者最大，死亡率終點的相對效果在高 eGFR 者更明顯。這恰恰是反對「人人同樣受益」單一敘事的最佳例證，也是「早用」的另一條理由線。

> **誠實邊界**：死亡率的顯著性依賴 **on-treatment 分析**與**猝死此一次要終點**；ITT 全因/CV 死亡未達顯著（P = 0.051／0.092）。講者**不宜**把它講成「finerenone 已證實降低死亡率」🔴 [stage4_ckd_Filippatos_2023]。

---

## 5. 誠實邊界（Evidence limits）🟡🔴

- Agarwal 2023、Bakris 2023、Filippatos 2023 均為 **FIDELITY 的 prespecified exploratory／post hoc 次分析**，P 值未校正多重比較；熱圖事件率為**安慰劑組觀察值**，非隨機化對照 🟡。
- Bakris 2023 的 **UACR 30–<300 亞群不確定性高**（HR 0.94；CI 0.60–1.47）；低白蛋白尿族群不宜以點估計下強斷言 🔴 [stage4_ckd_Bakris_2023]。
- Filippatos 2023 死亡率顯著性依賴 **on-treatment**＋**猝死次要終點**；ITT 未達顯著 🔴 [stage4_ckd_Filippatos_2023]。
- Agarwal 2023 的 **NHANES 6.4M／38,359 事件**為模擬外推，依賴美國人口結構假設，非試驗實測 🟡 [stage4_ckd_Agarwal_2023]。
- 具體數字專屬 FIDELITY（FIDELIO＋FIGARO 合併）族群（median UACR 515、mean eGFR 57.6），外推至非白蛋白尿 CKD、HF 場景須保留 🔴。
- 本叢集**不**納入 abstract-only 的 Zhao 2026／Zuin 2026 數字。

---

## 📊 簡報數據參考（從原文圖／表擷取）

> 用途：以下表格為「可直接貼進投影片」的乾淨版，每列標明來源檔＋grep 命中行號（行號依本地 MD 檔）。數字均逐字擷取自 fulltext 表/圖；**顏色概念一律是：數字（事件率）愈大 = 絕對事件率愈高 = 同一相對效果下 NNT 愈小 = 愈值得早用**。

### 📊 表 A — 熱圖：基線 eGFR×UACR 的絕對複合心血管事件率（安慰劑組，每 100 人年）

> 來源：`stage4_ckd_Agarwal_2023.md`，表格 grep 行 40–46（摘要重複值於行 28）。這是「who-to-treat-first」最核心的一張地形圖。

| eGFR（mL/min/1.73m²）↓ ＼ UACR → | UACR <300 mg/g | UACR ≥300 mg/g |
|---|---|---|
| **≥90** | 2.38 (1.03–4.29) | 3.78 (2.91–4.75) |
| **60–<90** | 3.57 (2.77–4.48) | 4.76 (4.11–5.45) |
| **45–<60** | 4.53 (3.72–5.42) | 5.70 (4.79–6.70) |
| **30–<45** | 4.93 (4.00–5.95) | 6.03 (5.14–6.99) |
| **<30** | 6.54 (4.19–9.40) | **8.74 (6.78–10.93)** |

- 整體療效：HR **0.86 (0.78–0.95)**，P = .002；eGFR×UACR **P-interaction = .66** → `stage4_ckd_Agarwal_2023.md` 行 52（摘要行 28）。
- 公衛尺度：模擬預防 **38,359** 件/年，**66%（25,357/38,360）**發生於 eGFR ≥60 → `stage4_ckd_Agarwal_2023.md` 行 56（摘要行 28）。

### 📊 表 B — 森林圖：腎臟複合終點（含 ≥57% eGFR 下降）by 基線 eGFR/UACR 分層

> 來源：`stage4_ckd_Bakris_2023.md`。Table（HR＋每 100 人年事件率）grep 行 199–206；Figure 3 森林圖（by 基線 eGFR 四層）grep 行 301–306。

| 分層 | Finerenone n/N | Placebo n/N | HR (95% CI) | P-interaction | 來源行號 |
|---|---|---|---|---|---|
| 整體腎臟複合 | 360/6519 | 465/6507 | 0.77 (0.67–0.88) | — | 行 199 / 21 / 63 |
| eGFR ≥60 | 90/2603 | 130/2592 | 0.70 (0.53–0.92) ⚠ | 0.62 | 行 200–201 |
| eGFR 45–<60 | 62/1717 | 87/1717 | 0.72 (0.52–1.00) | — | 行 202 |
| eGFR 25–<45 | 188/2117 | 225/2115 | 0.83 (0.68–1.01) | — | 行 203 |
| UACR 30–<300 | 38/2076 | 40/2023 | 0.94 (0.60–1.47) | 0.67 | 行 205 |
| UACR ≥300 | 321/4321 | 424/4371 | 0.75 (0.65–0.87) | — | 行 206 |

> ⚠ **來源表格擷取校正註**：`stage4_ckd_Bakris_2023.md` 行 199–206 的表格於 PDF→Markdown 轉檔時**欄位上移一列**（HR 與 IR 欄錯位），故 eGFR ≥60 列的 HR **0.70 (0.53–0.92)** 在原始 MD 中顯示於上一行（「Baseline eGFR」標題列），而該列位置實際落的「1.66 (1.38–1.95)」為 IR（每 100 人年事件率）而非 HR。判定 0.70 為正解之依據：事件數 90/2603（3.5%）vs 130/2592（5.0%），finerenone 事件**較少**，HR 必 <1，不可能為 1.66。做簡報時建議回原始 Kidney International Table 1 二次核對此格。

**Figure 3 森林（by 基線 eGFR，含事件率/100PY）** → `stage4_ckd_Bakris_2023.md` 行 303–306：

| 基線 eGFR | Finerenone n/N (IR) | Placebo n/N (IR) | HR (95% CI) | 來源行號 |
|---|---|---|---|---|
| <30 | 94/440 (8.80) | 92/450 (8.73) | 不可計算（PH 假設不成立）ᵃ | 行 303 |
| 30–<60 | 176/3475 (1.89) | 243/3463 (2.61) | 0.72 (0.59–0.88) | 行 304 |
| 60–<90 | 77/1944 (1.30) | 102/1932 (1.74) | 0.78 (0.57–1.05) | 行 305 |
| ≥90 | 13/659 (0.66) | 28/660 (1.40) | 0.44 (0.22–0.86) | 行 306 |

ᵃ 原文 Figure 3 註：eGFR <30 之 HR 因 Cox proportional hazards 假設不成立而未計算（`stage4_ckd_Bakris_2023.md` 行 326）；但兩組事件率同為 ~8.7–8.8/100PY，凸顯此族群**絕對事件率最高**。

- 腎臟分項：ESKD HR **0.80 (0.64–0.99)**；≥57% eGFR 下降 HR **0.70 (0.60–0.83)** → 行 63。
- 3 年 ARR **1.7% (0.7–2.6)**，NNT **60 (38–142)** → 行 63。

### 📊 表 C — 低 eGFR 的血鉀「取捨」數字（Table 2 安全性 by 基線 eGFR）

> 來源：`stage4_ckd_Bakris_2023.md`。文字敘述 grep 行 214；Table 2 grep 行 398–402。

| 安全終點 | eGFR <60：Fin vs Pbo | eGFR ≥60：Fin vs Pbo | 來源行號 |
|---|---|---|---|
| 因高血鉀停藥 | 2.4% vs 0.8% | 0.6% vs 0.3% | 行 214 / 400 |
| 高血鉀致住院 | 1.4% vs 0.3% | 0.3% vs 0% | 行 214 / 399 |
| 中央實驗室 K⁺ >5.5 | 20.5% vs 8.7% | 11.2% vs 5.4% | 行 401 |
| 中央實驗室 K⁺ >6.0 | 4.2% vs 1.3% | 1.9% vs 1.2% | 行 402 |

> 投影片訊息：**受益最大的低 eGFR 族群，血鉀停藥率也最高（2.4% vs 0.6%）**——這是「層級化取捨」，要配對監測節奏，不是不用的理由。

### 📊 表 D — 死亡率：ITT vs On-treatment 的「顯著性翻轉」

> 來源：`stage4_ckd_Filippatos_2023.md`，正文 grep 行 77 / 79 / 83；Key data points grep 行 128–136。

| 終點 | 分析 | Fin vs Pbo | HR (95% CI) | P | 來源行號 |
|---|---|---|---|---|---|
| 全因死亡 | ITT | 8.5% vs 9.4% | 0.89 (0.79–1.00) | 0.051 | 行 77 / 128 |
| 全因死亡 | On-treatment | 4.3% vs 5.3% | 0.82 (0.70–0.96) | 0.014 | 行 79 / 130 |
| CV 死亡 | ITT | 4.9% vs 5.6% | 0.88 (0.76–1.02) | 0.092 | 行 77 / 129 |
| CV 死亡 | On-treatment | 2.9% vs 3.6% | 0.82 (0.67–0.99) | 0.040 | 行 79 / 131 |
| 猝死 (SCD) | ITT | 1.3% (0.44/100PY) vs 1.8% (0.58/100PY) | 0.75 (0.57–0.996) | 0.046 | 行 83–84 / 132 |

- KDIGO 風險組人數：low **64**、moderate **1323**、high **5345**、very high **6288** → 行 91 / 134。
- 死亡率無 KDIGO 交互：全因 P-int **0.1293**、CV P-int **0.6361**；效果「more pronounced in patients with higher baseline eGFR」→ 行 93 / 135–136、行 29/39。

### 📊 表 E — 相對 vs 絕對：同一相對折扣、不同 NNT（含方法學錨點）

> 用途：一張投影片講完全篇邏輯。整體 NNT 來自 `stage4_ckd_Agarwal_2022.md`（grep 行 43、52）；方法學錨點來自 `subgroup_methodology_Sun_2010.md`（grep 行 44、46）。

| 項目 | 相對效果 | 絕對受益 / NNT | 來源行號 |
|---|---|---|---|
| FIDELITY 整體 · 複合 CV | HR 0.86 | NNT 46 (29–109) | `stage4_ckd_Agarwal_2022.md` 行 43 |
| FIDELITY 整體 · 複合腎臟 | HR 0.77 | 3 年 ARR 1.7% (0.7–2.6)；NNT 60 (38–142) | `stage4_ckd_Bakris_2023.md` 行 21 / 63 |
| 方法學：statin 低危 | RRR 29.2%（一致） | ARR 1.5%（5%→3.5%） | `subgroup_methodology_Sun_2010.md` 行 44 |
| 方法學：statin 高危 | RRR 29.2%（一致） | ARR 14.6%（50%→35.4%） | `subgroup_methodology_Sun_2010.md` 行 44 |

> 一句話讀圖：相對折扣一樣，NNT 卻由基線事件率決定——「absolute risk reduction ... must exist」（Sun 2010，行 46）。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|------|------|------------------|
| 相對一致 → 絕對受益必放大（方法學地基） | 🟡 方法學 | `subgroup_methodology_Sun_2010` 📄 |
| eGFR×UACR 絕對事件率梯度 2.38→8.74（安慰劑組） | 🟡 exploratory | `stage4_ckd_Agarwal_2023` 📄 |
| finerenone CV 療效不隨梯度改變（HR 0.86，P-int .66） | 🟡 exploratory | `stage4_ckd_Agarwal_2023` 📄 |
| 66% 可預防事件在 eGFR ≥60（公衛尺度） | 🟡 模擬外推 | `stage4_ckd_Agarwal_2023` 📄 |
| 腎臟複合 ↓23%（HR 0.77）、3 年 ARR 1.7%、NNT 60 | 🟡 pooled | `stage4_ckd_Bakris_2023`／`stage4_ckd_Agarwal_2022` 📄 |
| 腎臟終點跨 eGFR/UACR 方向一致（P-int 0.62/0.67） | 🟡 exploratory | `stage4_ckd_Bakris_2023` 📄 |
| UACR 30–<300 亞群不確定性高（HR 0.94；0.60–1.47） | 🔴 邊界 | `stage4_ckd_Bakris_2023` 📄 |
| 低 eGFR 受益最大、血鉀停藥率也最高（2.4% vs 0.6%） | 🟡 pooled | `stage4_ckd_Bakris_2023` 📄 |
| 死亡率 on-treatment 顯著、ITT 邊緣（HR 0.82 vs 0.89） | 🔴 on-treatment 依賴 | `stage4_ckd_Filippatos_2023` 📄 |
| 死亡率在高 eGFR 更明顯（不同終點最佳族群不同） | 🟡 exploratory | `stage4_ckd_Filippatos_2023` 📄 |
| 「梯度 → hard-outcome 個人化 NNT」之前瞻驗證 RCT | 🔴 尚無 | —（誠實揭露） |

## 本地全文語料（可 grep 稽核）

📄 全文：`stage4_ckd_Agarwal_2023`（JAMA Cardiol，eGFR×UACR 可修飾性熱圖）、`stage4_ckd_Bakris_2023`（Kidney Int，FIDELITY 腎臟 exploratory＋森林圖＋Table 2 安全性）、`stage4_ckd_Filippatos_2023`（EHJ-CVP，FIDELITY 死亡率＋KDIGO 分層）、`subgroup_methodology_Sun_2010`（BMJ，相對 vs 絕對 subgroup 準則）、`stage4_ckd_Agarwal_2022`（FIDELITY 整體 NNT）。

---

## References（Vancouver + [檔名]）

1. Agarwal R, Pitt B, Rossing P, Anker SD, Filippatos G, Ruilope LM, et al. Modifiability of composite cardiovascular risk associated with chronic kidney disease in type 2 diabetes with finerenone. JAMA Cardiol. 2023;8(8):732–41. doi:10.1001/jamacardio.2023.1505. 📄 [stage4_ckd_Agarwal_2023]
2. Bakris GL, Ruilope LM, Anker SD, Filippatos G, Pitt B, Rossing P, et al. A prespecified exploratory analysis from FIDELITY examined finerenone use and kidney outcomes in patients with chronic kidney disease and type 2 diabetes. Kidney Int. 2023;103(1):196–206. doi:10.1016/j.kint.2022.08.040. 📄 [stage4_ckd_Bakris_2023]
3. Filippatos G, Anker SD, August P, Coats AJS, Januzzi JL, Mankovsky B, et al. Finerenone and effects on mortality in chronic kidney disease and type 2 diabetes: a FIDELITY analysis. Eur Heart J Cardiovasc Pharmacother. 2023;9(2):183–91. doi:10.1093/ehjcvp/pvad001. 📄 [stage4_ckd_Filippatos_2023]
4. Sun X, Briel M, Walter SD, Guyatt GH. Is a subgroup effect believable? Updating criteria to evaluate the credibility of subgroup analyses. BMJ. 2010;340:c117. doi:10.1136/bmj.c117. 📄 [subgroup_methodology_Sun_2010]
5. Agarwal R, Filippatos G, Pitt B, Anker SD, Rossing P, Joseph A, et al. Cardiovascular and kidney outcomes with finerenone in patients with type 2 diabetes and chronic kidney disease: the FIDELITY pooled analysis. Eur Heart J. 2022;43(6):474–84. doi:10.1093/eurheartj/ehab777. 📄 [stage4_ckd_Agarwal_2022]

---
*此檔為主題四叢集一之延伸拆解，撰寫日期基準 2026-07-11。所有具體數字均可 grep 回上列本地全文 MD。本叢集全部四份主來源為本地全文（📄）；核心結論「相對一致→絕對放大→who-to-treat-first」為方法學＋prespecified/exploratory 次分析支撐（代理與觀察性成分見誠實邊界）；死亡率顯著性依賴 on-treatment 分析；「梯度→個人化 hard-outcome NNT」之前瞻驗證 RCT 目前不存在，屬明示之研究缺口。*
