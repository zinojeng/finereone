# 高血鉀的工程學：把風險按場景與環節拆開（研究設計、eGFR、SGLT2i、併用藥、baseline K⁺）

> 本文為主題五（高血鉀與 eGFR dip 的安全工程學）之延伸拆解，把主文「表 5」那一節從一張並列表，展開成**三個拆解維度**：按**臨床場景**拆、按**研究設計**拆、按**風險修飾因子（環節）**拆。核心命題只有一句——**finerenone 的高血鉀「風險」不是單一數字，而是隨研究型態、eGFR、baseline K⁺、併用藥而變的一組數字**；把它們拆開，「相對風險約 2 倍、絕對硬結局低」才會從口號變成可操作的門診決策。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（不對其未載內容作具體數字斷言）。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織與改寫，所有作者／年份／數字均出自本地 MD 檔。
>
> **證據分層**：🟢 guideline routine（已進指引常規）｜🟡 evidence expansion（post hoc／次分析／surrogate／IPD pooled）｜🔴 尚待驗證（無對應 hard-outcome RCT，或屬尚未定稿草案）。

---

## 0. 一句話定位

同一顆藥，在不同「切法」下高血鉀數字差很多：**整體 pooled 約 14%、進階 CKD 單試驗約 21%、Stage 4 亞群約 26%、心衰場景反而約 10%、合併 SGLT2i 不放大甚至略降**。差異不是矛盾，而是「風險被什麼修飾」的訊號。要回答「風險可不可管理」，就得先承認它**不是一個數字**，再逐環節拆給病人與團隊看。

---

## 1. 按場景拆：同一藥、六種切法、六組數字

### 表 A. 各場景的高血鉀事件率、住院率、永久停藥率（finerenone vs 安慰劑）

| 場景（研究型態） | 高血鉀事件 | 住院（高血鉀） | 永久停藥（高血鉀） | 主要本地來源 |
|---|---|---|---|---|
| **FIDELITY pooled**（CKD+T2D，>13,000；prespecified pooled） | 14.0% vs 6.9% | 0.9% vs 0.2% | 1.7% vs 0.6% | [label_guideline_safety_European_2022] 📄 |
| — 實驗室 K⁺ >5.5 / >6.0 | 16.8% vs 7.4% / 3.3% vs 1.3% | — | — | [label_guideline_safety_European_2022] 📄 |
| **FIDELIO-DKD**（進階 CKD 單試驗；post hoc 安全分析） | ≥mild(>5.5) 21.4% vs 9.2%；≥mod(>6.0) 4.5% vs 1.4% | — | 藥物撤除 2.3% vs 0.9% | [pooled_safety_hyperkalemia_Agarwal_2022] 📄 |
| **Stage 4 CKD 亞群**（eGFR<30，n=890；亞群 post hoc） | 26% vs 13% | 3% vs 1% | 3% vs 2% | [pooled_safety_hyperkalemia_Sarafidis_2023] 📄 |
| **FINEARTS-HF**（HFmrEF/HFpEF；RCT 主終點＋次分析） | 9.7% vs 4.2% | 0.5% vs 0.2% | 0.4% vs 0.2% | [label_guideline_safety_European_2022] 📄 |
| **CONFIDENCE combo**（very-high risk 亞群；三臂 Phase 2） | AE 13.5%(combo)/11.4%(fine)/5.1%(empa) | — | — | [hf_renal_safety_Vaduganathan_2025] 📄 |
| **INFINITY IPD**（FIDELIO+FIGARO+FIND-CKD，n=14,574；prespecified IPD） | 14·3% vs 7·6% | 0·9% vs 0·2% | 1·7% vs 0·5% | [pooled_safety_hyperkalemia_Neuen_2026] 📄 |
| **FINE-HEART IPD**（FIDELIO+FIGARO+FINEARTS-HF 糖尿/CKD 亞群，n=14,180；prespecified IPD） | 實驗室 K>5.5 18% vs 8% | 1% vs 0.2% | 2% vs 1% | [hf_renal_safety_Ostrominski_2026] 📄 |

> **讀表要領**：這六（八）列**不能直接互比絕對數字**，因為分母、事件定義（investigator-reported vs 中央實驗室 K⁺ 閾值）、追蹤長度、族群風險都不同。它們的**共同不變量**是方向與量級——相對約 2 倍、絕對硬結局低、幾乎零高血鉀死亡。

### 1.1 進階 CKD 單試驗（FIDELIO-DKD）：把風險量化得最完整

FIDELIO-DKD 的 post hoc 安全分析（中位追蹤 **2.6 年**）中，≥mild 高血鉀 **597/2785（21.4%）** vs **256/2775（9.2%）**、≥moderate(>6.0) **126/2802（4.5%）** vs **38/2796（1.4%）** [pooled_safety_hyperkalemia_Agarwal_2022] 📄。處置以「暫時撤藥」為主：藥物**中斷** finerenone **310（11.0%）** vs placebo 146（5.2%）、藥物**撤除** 64（2.3%）vs 25（0.9%）[pooled_safety_hyperkalemia_Agarwal_2022] 📄。多變量校正後 finerenone 對 ≥mild 高血鉀的獨立 **HR 2.13（1.86–2.45），P<0.0001**——這就是「相對約 2 倍」在單試驗層級的錨點 [pooled_safety_hyperkalemia_Agarwal_2022] 📄。

### 1.2 Stage 4 亞群（eGFR<30）：發生率翻倍，但停藥仍溫和

Stage 4 亞群共 **890（7%）**，平均 eGFR **26.9**、中位 UACR 720 mg/g [pooled_safety_hyperkalemia_Sarafidis_2023] 📄。高血鉀 **26% vs 13%**（翻倍），但永久停藥僅 **3% vs 2%**、住院 **3% vs 1%**、**無高血鉀死亡** [pooled_safety_hyperkalemia_Sarafidis_2023] 📄。血鉀變化溫和：月 4 平均變化 **0.26（SD 0.51）** vs 0.02（SD 0.49），其後平穩 [pooled_safety_hyperkalemia_Sarafidis_2023] 📄。同時此亞群保有心腎益處：CV composite **HR 0.78（0.57–1.07）**、chronic eGFR slope 由 **−3.2 改善至 −1.8 mL/min/年（差 1.39；0.48–2.30；P=0.04）**、UACR 月 4 降 **31%** [pooled_safety_hyperkalemia_Sarafidis_2023] 📄。（誠實邊界：kidney composite 之比例風險假設在 2 年後不成立，作者標為 exploratory [pooled_safety_hyperkalemia_Sarafidis_2023] 📄。）

### 1.3 心衰場景（FINEARTS-HF）：高血鉀反而較輕

HFmrEF/HFpEF 的高血鉀**絕對**發生率反而低（9.7% vs 4.2%）、永久停藥極低（0.4% vs 0.2%）[label_guideline_safety_European_2022] 📄。Vardeny 次分析：K⁺ >5.5 **HR 2.16（1.83–2.56）**、>6.0 **HR 2.07（1.4–3.0）**、K⁺ <3.5 **HR 0.46（0.38–0.56）**（雙向，見同資料夾 `hypokalemia_bidirectional_electrolyte.md`）[hf_renal_safety_Vardeny_2025] 📄。跨劑量一致：20-mg 層 HR **2.02（1.63–2.50）**、40-mg 層 HR **2.35（1.80–3.05）**，interaction P=.39 [hf_renal_safety_Vardeny_2025] 📄。**關鍵**：即使第 1 個月即升至 >5.5，finerenone 的臨床益處仍維持——經歷 vs 未經歷 K⁺ >5.5 的療效 **HR 0.84（0.55–1.30）vs 0.83（0.74–0.92），interaction P=.72** [hf_renal_safety_Vardeny_2025] 📄。

### 1.4 兩份 2026 IPD pooled：把結論延伸到更廣 CKD 譜

- **INFINITY**（n=**14 574**，首度納入**非糖尿病 CKD**／FIND-CKD）：任一高血鉀 **14·3%（1043）vs 7·6%（553）**、永久停藥 **1·7%（122）vs 0·5%（39）**、serious **1·1%（77）vs 0·3%（21）**、住院 **0·9%（68）vs 0·2%（15）**、life-threatening **0·1% vs 0·1%**、fatal **0 vs 0**；實驗室 K>5.5 **17·0% vs 7·9%**、K<3.5 3·6% vs 8·0%；作者明示**無任何可歸因於高血鉀之死亡** [pooled_safety_hyperkalemia_Neuen_2026] 📄。
- **FINE-HEART**（n=**14,180**，FINEARTS-HF 糖尿/CKD 亞群併入）：實驗室 K>5.5 **18% vs 8%**、K>6.0 **4%**、永久停藥 **2% vs 1%**、住院 **1%（69）vs 0.2%（15）**、**無高血鉀死亡**；SAE 反而 finerenone 較低（**34% vs 36%**）。把絕對可管理性量成一個門診好記數字：每處方約 **131** 人才造成 1 次高血鉀相關住院（NNT=131）[hf_renal_safety_Ostrominski_2026] 📄。同一分析 CV death/HHF **HR 0.83（0.75–0.93）**、NNT 60 [hf_renal_safety_Ostrominski_2026] 📄。

---

## 2. 按研究設計拆：為什麼「相對約 2 倍」與「絕對很低」可以並存

「風險大不大」的答案取決於你在看哪種設計、哪個分子分母：

- **相對風險（約 2 倍）** 來自把「事件率」相除——它對族群基礎風險不敏感，因此在 pooled、單試驗、亞群、IPD 各層級都穩定落在 ~2×。
- **絕對事件（住院、永久停藥、死亡）** 來自把「臨床相關重症」當分子——它們在各場景都低（住院 <1%～3%、永久停藥 0.4%～3%、死亡 0），因為**協議化的監測＋暫停/減量把重症攔截掉了**。

### 2.1 KDIGO 2026 為此更新做的 7-study 統合（🟡，尚未定稿草案）

**KDIGO 2026 糖尿病與 CKD 指引更新・公開審查草案**為此次更新做的新統合（**7 studies、41 reports**、nsMRA[finerenone 或 esaxerenone] vs placebo、T2D+CKD、全數排除 eGFR<25）量化了「風險真實但可量化」：hyperkalemia（未細分）**RR 2.09（95% CI 1.82–2.39）**、serum potassium ≥5.5 mmol/l **RR 2.18（95% CI 1.98–2.40）** [KDIGO_2026_Diabetes_CKD_draft] 📄。同一統合中療效**顯著**：kidney composite **HR 0.84（0.77–0.92）**、kidney failure **HR 0.84（0.71–0.99）**、HF/HHF **HR 0.78（0.66–0.92）**；而 all-cause mortality **RR 0.90（0.81–1.00）**、CV mortality **RR 0.88（0.76–1.02）**、stroke **RR 1.01（0.83–1.22）**、nonfatal MI **RR 0.92（0.75–1.13）** 未達顯著 [KDIGO_2026_Diabetes_CKD_draft] 📄。草案並記載 kidney failure／HHF／kidney composite 三項的證據確定性為 **high** [KDIGO_2026_Diabetes_CKD_draft] 📄。（誠實邊界：此為**公開審查草案、尚未定稿** 🔴🟡；Chapter 4。）

### 2.2 相對 2 倍在各設計的一致性（可交叉核對）

| 設計層級 | 相對指標 | 數值 | 來源 |
|---|---|---|---|
| 7-study 統合（含 esaxerenone） | hyperkalemia RR | 2.09（1.82–2.39） | [KDIGO_2026_Diabetes_CKD_draft] 📄 |
| 7-study 統合 | K≥5.5 RR | 2.18（1.98–2.40） | [KDIGO_2026_Diabetes_CKD_draft] 📄 |
| FIDELIO 單試驗多變量 | finerenone HR | 2.13（1.86–2.45） | [pooled_safety_hyperkalemia_Agarwal_2022] 📄 |
| FINEARTS-HF 次分析 | K>5.5 HR | 2.16（1.83–2.56） | [hf_renal_safety_Vardeny_2025] 📄 |

三種完全不同的設計（統合／單試驗多變量／HF 次分析）給出 2.09／2.13／2.16——**相對約 2 倍是穩健事實**；差異全在「絕對事件」層。

---

## 3. 按環節拆：風險修飾因子（本節最重要的「工程學」）

FIDELIO 多變量 Cox 把「哪些環節推高／壓低風險」列成一張可操作清單。以下 HR 皆為 ≥mild 高血鉀之獨立預測因子 [pooled_safety_hyperkalemia_Agarwal_2022] 📄：

| 修飾因子（環節） | HR（95% CI） | 方向 |
|---|---|---|
| baseline K⁺ >5.0（vs 4.1–4.5） | **4.18（3.45–5.05）** | ⬆ 最強 |
| baseline K⁺ 4.8–5.0 | 2.78（2.25–3.44） | ⬆ |
| baseline K⁺ 4.5–4.8 | 1.53（1.29–1.82） | ⬆ |
| baseline K⁺ ≤4.1 | 0.44（0.35–0.55） | ⬇（低起點保護） |
| eGFR <25（vs ≥60） | **2.04（1.35–3.07）** | ⬆ |
| eGFR 25–<45 | 1.51（1.19–1.91） | ⬆ |
| eGFR 45–<60 | 1.02（0.80–1.32） | ≈ |
| 每倍 UACR（log2） | 1.12（1.07–1.17） | ⬆ 輕 |
| β-blocker（用 vs 不用） | **1.18（1.04–1.35）** | ⬆ 輕 |
| 利尿劑（用 vs 不用） | **0.76（0.66–0.87）** | ⬇ |
| SGLT2i（用 vs 不用） | **0.45（0.27–0.75）** | ⬇ 最強 |
| ACEi/ARB 劑量（各層） | 不顯著（P=0.8508） | ≈ |

> **操作含義**：這張表就是「選對病人＋調對背景藥」的清單——**baseline K⁺ 與 eGFR 是最大槓桿**（起始前把 K⁺ 控在 ≤5.0、eGFR ≥25）；**SGLT2i 與利尿劑是內建的降鉀夥伴**；β-blocker 是隱形的升鉀因子（不是禁忌，是監測訊號）。

### 3.1 eGFR 分層的絕對事件（Bakris FIDELITY 安全分析，新增細節）

同一 eGFR 環節在絕對事件也看得到、但仍低 [pooled_safety_hyperkalemia_Bakris_2023] 📄：

- 任一 investigator-reported 高血鉀：eGFR<60 **714（18.3%）vs 333（8.5%）**；eGFR≥60 **198（7.6%）vs 115（4.4%）**。
- 因高血鉀**永久停藥**：eGFR<60 **2.4% vs 0.8%**；eGFR≥60 **0.6% vs 0.3%**。
- 因高血鉀**住院**：eGFR<60 **1.4% vs 0.3%**；eGFR≥60 **0.3% vs 0%**。

即使 eGFR<60、發生率近 2 倍，永久停藥仍在個位數低百分比——**低 eGFR 是「監測更勤」的訊號，不是禁忌**（呼應 EMA「eGFR<60 與高齡者更頻繁監測」[label_guideline_safety_European_2022] 📄）。

### 3.2 併用 SGLT2i / GLP-1RA：未放大高血鉀（多來源一致）

- **CONFIDENCE combo（very-high risk 亞群）**：AE 高血鉀 combo **13.5%** vs finerenone **11.4%** vs empagliflozin **5.1%**（total 10.0%）；實驗室 K⁺ >5.5 combo **19.6%** vs finerenone **22.3%** vs empagliflozin **10.3%**（total 17.3%）——作者明言合併治療各 KDIGO 風險層的高血鉀率**在數值上都比 finerenone 單藥略低** [hf_renal_safety_Vaduganathan_2025] 📄。方向與 FIDELIO 次分析 SGLT2i 使用者 HR 0.45 一致 [pooled_safety_hyperkalemia_Agarwal_2022] 📄。
- **合併 GLP-1RA（CONFIDENCE 次分析，n=800，182[23%] 用 GLP-1RA）**：combo 高血鉀率有／無 baseline GLP-1RA 者為 **9.0% 與 9.5%**，幾乎相同 [hf_renal_safety_Agarwal_2025] 📄。
- **FIDELITY SGLT-2i／GLP-1RA 次分析**（子群：combined SGLT-2i+GLP-1RA **n=167**、皆無 **n=11,341**、SGLT-2i only **n=706**、GLP-1RA only **n=776**）：明言「finerenone 的安全輪廓不因併用 SGLT-2i 和／或 GLP-1RA 而改變；導致停藥或住院的高血鉀事件低」[pooled_safety_hyperkalemia_Singh_2026] 📄。

> **誠實邊界（重要，不可只講一面）**：Vaduganathan 的「combo 數值略低」是**KDIGO 風險層次分析**的觀察；但 KDIGO 2026 草案在敘述整體 CONFIDENCE 時明白寫道「**the addition of empagliflozin to finerenone did not appear to mitigate the effect of hyperkalemia with an nsMRA**」（合併 empagliflozin 並未「消除」nsMRA 的高血鉀）[KDIGO_2026_Diabetes_CKD_draft] 📄。正確的門診話術是：**併用 SGLT2i「不放大、甚至數值略降」高血鉀，但不能倚賴它「抵銷」——監測仍不可省**。combination 的效益證據以 UACR 為代理終點（day 180 combo 較 finerenone 單藥多降 **29%**，LSM ratio **0.71（0.61–0.82）**；較 empagliflozin 單藥多降 **32%**，**0.68（0.59–0.79）**）[KDIGO_2026_Diabetes_CKD_draft] 📄，屬 surrogate-based evidence expansion 🟡，非心腎硬終點 🔴。KDIGO 2026 已據此新增 **Practice Point 4.4.2**（SGLT2i 與 nsMRA 可同步起始）[KDIGO_2026_Diabetes_CKD_draft] 📄。

---

## 4. 血鉀動力學：為什麼「可回收」

三個動力學事實，解釋為何相對 2 倍不轉成重症：

1. **幅度小且平台化**：finerenone 造成的組間平均差**最大僅 0.23 mmol/L（月 4）**，其後穩定 [pooled_safety_hyperkalemia_Agarwal_2022] 📄；EMA 記載首月平均升幅 **≤0.2 mmol/L** 後即穩定 [label_guideline_safety_European_2022] 📄。
2. **短半衰期、無活性代謝物**：CKD 中半衰期 **2–3 小時**、無活性代謝物，故高血鉀可藉暫停治療處理 [label_guideline_safety_Wanner_2022] 📄 [pooled_safety_hyperkalemia_Agarwal_2022] 📄。協議做法：K⁺ >5.5 暫停、待 ≤5.0 再以 10 mg 重啟 [label_guideline_safety_Wanner_2022] 📄。
3. **「可回收」的機制學證據**：FIDELIO spline 顯示月 4 時，同樣 0.5 mmol/L 的血鉀上升，**安慰劑對應 ~3.4 倍**後續高血鉀風險、**finerenone 僅 ~twofold**（組間差異 P=0.011）[pooled_safety_hyperkalemia_Agarwal_2022] 📄——暗示 finerenone 的短半衰期使其高血鉀比長效 steroidal MRA 更易回收。

Wanner 的實務綜述總結：>13,000 病人、中位追蹤 3 年，**無任何可歸因於高血鉀的死亡** [label_guideline_safety_Wanner_2022] 📄；INFINITY／FINE-HEART／Stage 4 亞群亦一致零高血鉀死亡 [pooled_safety_hyperkalemia_Neuen_2026] 📄 [hf_renal_safety_Ostrominski_2026] 📄 [pooled_safety_hyperkalemia_Sarafidis_2023] 📄。

---

## 5. 誠實邊界（Evidence limits）

- **設計性質差異**：FIDELIO/Bakris/Agarwal 為**單試驗 post hoc**；Sarafidis 為**亞群 post hoc**（kidney composite 屬 exploratory）；Vardeny/Vaduganathan/Agarwal_2025/Singh 為**次分析／亞群**；Neuen/Ostrominski 為**prespecified IPD pooled**；KDIGO 7-study 統合為**尚未定稿的公開審查草案**。相對 2 倍穩健，但**跨場景絕對數字不可直接互比**（分母、事件定義、追蹤長度不同）。
- **combination 論述**：以 UACR 為 surrogate 主終點 🟡；「combo 不放大高血鉀」是次分析／風險層觀察，**KDIGO 明言未『消除』高血鉀** 🔴——監測不可省。
- **無 binder-enabled finerenone 硬終點 RCT** 🔴：見同資料夾 `potassium_binder_role.md`。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|------|------|------------------|
| 相對風險約 2 倍（RR 2.09、K≥5.5 RR 2.18；7-study 統合） | 🟡（尚未定稿草案） | `KDIGO_2026_Diabetes_CKD_draft` 📄 |
| 單試驗多變量 finerenone HR 2.13、修飾因子清單 | 🟡 post hoc | `pooled_safety_hyperkalemia_Agarwal_2022` 📄 |
| Stage 4 亞群 26% vs 13%、停藥 3% vs 2%、CV HR 0.78 | 🟡 亞群 post hoc | `pooled_safety_hyperkalemia_Sarafidis_2023` 📄 |
| 心衰場景高血鉀較輕、療效不被中度升鉀抵銷（interaction P=.72） | 🟡 次分析 | `hf_renal_safety_Vardeny_2025` 📄 |
| IPD pooled 延伸至非糖尿 CKD／HF、零高血鉀死亡、NNH 20／NNT 131 | 🟡 prespecified IPD | `pooled_safety_hyperkalemia_Neuen_2026`、`hf_renal_safety_Ostrominski_2026` 📄 |
| 併用 SGLT2i/GLP-1RA 未放大高血鉀（但未『消除』） | 🟡 次分析／草案 | `hf_renal_safety_Vaduganathan_2025`、`_Agarwal_2025`、`pooled_safety_hyperkalemia_Singh_2026`、`KDIGO_2026_Diabetes_CKD_draft` 📄 |
| 血鉀「可回收」（≤0.23 mmol/L、半衰期 2–3 h、零死亡） | 🟢🟡 | `label_guideline_safety_European_2022`、`_Wanner_2022`、`pooled_safety_hyperkalemia_Agarwal_2022` 📄 |
| combination → 心腎硬終點 RCT | 🔴 尚無 | —（研究缺口，誠實揭露） |

## 本地全文語料（可 grep 稽核）

📄 全文：`pooled_safety_hyperkalemia_Agarwal_2022`（FIDELIO post hoc）、`_Sarafidis_2023`（Stage 4 亞群）、`_Neuen_2026`（INFINITY IPD）、`_Singh_2026`（FIDELITY SGLT-2i/GLP-1RA 次分析）、`_Bakris_2023`（FIDELITY eGFR 分層安全）、`hf_renal_safety_Ostrominski_2026`（FINE-HEART IPD）、`_Vardeny_2025`（FINEARTS-HF 血鉀）、`_Vaduganathan_2025`（CONFIDENCE KDIGO 風險層）、`_Agarwal_2025`（CONFIDENCE GLP-1RA 次分析）、`_Green_2023`（CONFIDENCE 設計）、`label_guideline_safety_European_2022`（EMA SmPC）、`_Wanner_2022`（實務綜述）、`KDIGO_2026_Diabetes_CKD_draft`（7-study 統合／Practice Point 4.4.2，公開審查草案）。

---

## References（本地可稽核）

1. Agarwal R, Joseph A, Anker SD, et al. Hyperkalemia risk with finerenone: a post hoc analysis of FIDELIO-DKD. 📄 [pooled_safety_hyperkalemia_Agarwal_2022]
2. Sarafidis P, Agarwal R, Pitt B, et al. Outcomes with finerenone in participants with stage 4 CKD and type 2 diabetes: a FIDELITY subgroup analysis. 2023. 📄 [pooled_safety_hyperkalemia_Sarafidis_2023]
3. Neuen BL, et al. Efficacy and safety of finerenone in CKD: an individual participant data pooled analysis (INFINITY; FIDELIO-DKD+FIGARO-DKD+FIND-CKD, n=14,574). 2026. 📄 [pooled_safety_hyperkalemia_Neuen_2026]
4. Ostrominski JW, Vaduganathan M, et al. FINE-HEART pooled analysis of finerenone (FIDELIO-DKD+FIGARO-DKD+FINEARTS-HF, n=14,180). 2026. 📄 [hf_renal_safety_Ostrominski_2026]
5. Vardeny O, et al. Serum potassium derangements and outcomes with finerenone in HFmrEF/HFpEF: FINEARTS-HF. 2025. 📄 [hf_renal_safety_Vardeny_2025]
6. Vaduganathan M, et al. Simultaneous finerenone and empagliflozin across KDIGO risk categories (CONFIDENCE). 2025. 📄 [hf_renal_safety_Vaduganathan_2025]
7. Agarwal R, et al. Impact of baseline GLP-1 RA use on albuminuria and safety with simultaneous finerenone + empagliflozin (CONFIDENCE). Diabetes Care. 2025. 📄 [hf_renal_safety_Agarwal_2025]
8. Singh AK, Anker SD, Pitt B, et al. A FIDELITY analysis on finerenone with SGLT-2i and GLP-1RA in CKD. Kidney Int Rep. 2026;11:103704. 📄 [pooled_safety_hyperkalemia_Singh_2026]
9. Bakris GL, et al. Kidney outcomes and safety of finerenone by baseline eGFR: FIDELITY analysis. 2023. 📄 [pooled_safety_hyperkalemia_Bakris_2023]
10. Kidney Disease: Improving Global Outcomes (KDIGO). 2026 Clinical Practice Guideline for Diabetes Management in CKD — Public Review Draft (Chapter 4; 7-study nsMRA meta-analysis; Practice Point 4.4.2). 📄 [KDIGO_2026_Diabetes_CKD_draft]
11. European Medicines Agency. Kerendia (finerenone) Summary of Product Characteristics. 2022. 📄 [label_guideline_safety_European_2022]
12. Wanner C, et al. Practical potassium management with finerenone in CKD and T2D. 2022. 📄 [label_guideline_safety_Wanner_2022]
13. Green JB, et al. Design of the CONFIDENCE study (finerenone + empagliflozin, UACR endpoint). 2023. 📄 [hf_renal_safety_Green_2023]

---
*此檔為主題五之延伸拆解，撰寫日期基準 2026-07-11。所有具體數字均可 grep 回上列本地全文 MD；KDIGO 2026 為公開審查草案（尚未定稿）、combination 之心腎硬終點證據尚缺，均已明示標註。*
