# 叢集三 · HF 風險、LVH、基線治療目標達標度與胰島素阻抗

> 本檔為主題四（誰獲益最大）主文 §5「叢集三」之延伸拆解＋**簡報數據集**。把「HF 風險族群、左心室肥厚（LVH）、基線治療目標達標度、合併用藥脈絡、胰島素阻抗」五個子題，從主文的濃縮條列擴充成**門診口吻的白話解說＋可直接貼投影片的圖表數據**。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（status: abstract_only，**不對其未載內容作具體數字擴張**）。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織與改寫。
>
> **證據分層**：🟢 guideline routine（已進指引常規）｜🟡 evidence expansion（prespecified／post hoc／exploratory／代理終點）｜🔴 尚待驗證（無直接 hard-outcome RCT、或僅 abstract／機轉假說）。
>
> **一句話定位**：這一叢集回答的是「**哪些看起來『心臟／腎臟已經被顧到』或『控制得不錯』的病人，其實還在漏水**」——答案是：即使沒有 HF 病史、即使 BP/HbA1c/LDL 都達標，finerenone 仍在減少事件；而 LVH 這一個心臟結構訊號，可能標記出「HF 住院獲益特別大」的一群。

---

## 1. HF 風險：沒有 HF 病史的人，仍能「預防新發心衰竭」

### 1.1 這段為什麼重要（門診版）🟡

門診常見的直覺是：「這個病人沒有心衰竭病史，射血分數也正常，HF 不是我現在要煩惱的事。」FIGARO-DKD 的 HF 分析把這個直覺推翻——**全族群只有 7.8%（571/7352）有 HF 病史**，但 finerenone 在**完全沒有 HF 病史**的人身上，仍顯著減少了「第一次因心衰竭住院」這件事 [hf_kidney_spectrum_Filippatos_2022]。也就是說，這些病人不是「治療已存在的 HF」，而是**攔截 HF 的發生**（把 stage A/B 往 stage C 的進展踩剎車）。

### 1.2 數字 🟡

- **新發 HF**（無 HF 病史者第一次因 HF 住院）：finerenone 65/3396（1.9%）、事件率 0.57 per 100 patient-years vs placebo 95/3385（2.8%）、0.84 per 100 patient-years；**HR 0.68（95% CI 0.50–0.93；P=0.016）**；48 個月 ARR 1.1%、**NNT 91（49–605）** [hf_kidney_spectrum_Filippatos_2022]。
- **CV 死亡或首次 HHF**：HR 0.82（0.70–0.95；P=0.011），ARR 1.8%、**NNT 55（29–393）** [hf_kidney_spectrum_Filippatos_2022]。
- **首次 HHF**：HR 0.71（0.56–0.90；P=0.0043），ARR 1.4%、NNT 70（39–292） [hf_kidney_spectrum_Filippatos_2022]。
- **HF 死亡或首次 HHF**：HR 0.68（0.54–0.86；P=0.0013），ARR 1.7%、NNT 60（35–177） [hf_kidney_spectrum_Filippatos_2022]。
- **總 HHF（首次＋復發）**：rate ratio 0.70（0.52–0.94） [hf_kidney_spectrum_Filippatos_2022]。

### 1.3 「相對一致、絕對放大」在 HF 面向的實例 🟡

效果**不被 HF 病史修飾**（各 P for interaction 均不顯著，如 CV 死亡或首次 HHF 的 P_interaction=0.81） [hf_kidney_spectrum_Filippatos_2022]。但因為有 HF 病史者事件率高得多（CV 死亡或首次 HHF：有病史 54/290＝18.6% vs 無病史 236/3396＝6.7%），其**絕對受益約 3 倍**：48 個月 ARR **−4.8%（−13.7 to 4.1）有 HF 病史 vs −1.6%（−3.1 to 0.0）無病史** [hf_kidney_spectrum_Filippatos_2022]。

> **門診轉譯**：兩件事同時成立——(1) **沒有 HF 病史也值得用**（能防新發 HF，NNT 91）；(2) **已有 HF 病史者絕對受益最大、最該優先**（ARR 約 3 倍）。這正是 who-to-treat-first 的核心。

### 1.4 「有 HF 病史」次族群的統合證據（Jaiswal）🟡

Jaiswal 的統合分析（2 個 RCT、**1,007 名有 HF 病史者**：485 finerenone / 522 placebo，平均年齡 65.95±0.71）確認：**首次 HHF OR 0.68（0.47–0.98；P=0.04；I²=0%）**（降 32%），但**心血管複合終點非顯著（OR 0.79，0.60–1.04）**，**高血鉀 OR 2.16（1.38–3.38；P<0.001）** [hf_kidney_spectrum_Jaiswal_2024]。訊號方向與 FIGARO 一致：HF 住院是最穩的獲益，CV 複合因事件數少而未達顯著。

### 1.5 補充：HHF 是「最穩健」的心血管獲益（Zuin，abstract-only）📌🔴

Zuin 的 fragility 分析（status: abstract_only，僅 abstract 可稽核）指出：在 FIDELIO／FIGARO／FIDELITY 三者中，**HF 住院是唯一「最一致、最 robust」的心血管獲益**（FIDELITY HHF：HR 0.78、NNT 91、fragility index 23），而 CV 死亡／MI／stroke 的訊號較 fragile [baseline_goals_absolute_Zuin_2026]。**因屬 abstract-only，本檔不擴張其表內以外之數字。**

---

## 2. LVH：一個「效果修飾子」候選（森林圖重點）

### 2.1 白話：為什麼要看 LVH 🟡

左心室肥厚（LVH）是「心臟長期被高壓、被容量、被醛固酮驅動而變厚」的結構印記。理論上，一個直接對抗 MR 過度活化、能減少心肌纖維化的藥，應該在「心臟已經因 MR 過度活化而變厚」的人身上特別有用。Filippatos 2024 就是在 FIDELITY（**13,026 人，96.5% 有高血壓、9.6% ECG 診斷 LVH、7.7% 有 HF**）裡檢驗這件事 [hf_kidney_spectrum_Filippatos_2024]。

### 2.2 數字：整體終點沒有交互，但 HHF 出現顯著交互 🟡

- **整體 CV 複合**：LVH HR 0.72（0.55–0.95）vs 無 LVH HR 0.89（0.81–0.98），**P_interaction=0.1075（未達顯著）** [hf_kidney_spectrum_Filippatos_2024]。
- **整體腎臟複合**：LVH HR 0.56（0.38–0.84）vs 無 LVH HR 0.80（0.69–0.93），**P_interaction=0.1782（未達顯著）** [hf_kidney_spectrum_Filippatos_2024]。
- **HHF（心衰竭住院）**：LVH HR **0.34（0.19–0.61）** vs 無 LVH HR 0.86（0.72–1.03），**P_interaction=0.0024（顯著）** [hf_kidney_spectrum_Filippatos_2024]。

### 2.3 誠實邊界 🔴

作者把 LVH 定位為「HHF 效果的**預測因子（predictor）**」，而非「應該據此篩選病人」的效果修飾子；並坦承：ECG 判讀**無中央裁決、無標準化 LVH 準則、缺 echo 佐證、後期 ECG 資料缺失**，屬 **hypothesis-generating** 的 post hoc 分析 [hf_kidney_spectrum_Filippatos_2024]。這是全套次分析中少數 P_interaction<0.05 的訊號——依方法學文獻（單一顯著交互多需外部重現），仍應以懷疑態度對待。安全面：TE 高血鉀在 LVH 亞群 finerenone 12.3% vs placebo 5.7%、無 LVH 者 14.2% vs 7.0%，但**因高血鉀停藥率低**（LVH 1.5% vs 0.5%、無 LVH 1.7% vs 0.6%） [hf_kidney_spectrum_Filippatos_2024]。

---

## 3. 基線治療目標達標度：達標愈多、絕對風險愈低，但 finerenone 效益不因達標與否改變

### 3.1 白話：這一段顛覆「先控好再加藥」的直覺 🟡

門診常說：「先把血壓、糖化血色素、血脂壓好，SGLT2i／GLP-1RA 也上了，再看要不要加 finerenone。」Neves 2026（FIDELITY，依 ADA 四大目標：HbA1c ≤7.0%、BP <130/80、LDL <1.81 mmol/L、使用 SGLT2i/GLP-1RA）給的答案是——**不必等**。基線達 0/1/2/≥3 目標者分別佔 **29%（3732）/40%（5208）/24%（3091）/7%（959）**，**共 12,990 人** [baseline_goals_absolute_Neves_2026]。

### 3.2 兩個同時成立的事實 🟡

**(A) 達標愈多、基線絕對風險愈低**（安慰劑組心血管事件率 per 100 patient-years）：**6.0 / 5.1 / 4.3 / 3.5**（0/1/2/≥3 目標） [baseline_goals_absolute_Neves_2026]。這證明「控制愈好、風險愈低」是真的。

**(B) 但 finerenone 的相對效益不因達標與否改變**——各終點 P_interaction 均不顯著：CV（**P_interaction=0.7481**，整體 HR 0.86，0.78–0.95）、腎臟（**0.6095**，整體 HR 0.76，0.66–0.88）、HHF（**0.7288**，整體 HR 0.78，0.66–0.92）、全因死亡（**0.0659**，整體 HR 0.89，0.79–1.00） [baseline_goals_absolute_Neves_2026]。

> **關鍵臨床訊息**：即使病人已達成所有傳統治療目標，仍從 finerenone 獲益——**不應等到危險因子控制達標才加藥** [baseline_goals_absolute_Neves_2026]。反面同樣成立：**未達標者絕對事件率最高（6.0/100 patient-years）**，是絕對受益最大、最該早用的一群。

### 3.3 一個「勿以單一亞群點估計改寫判讀」的教學案例 🟡

Neves 的 ≥3 目標亞群，腎臟終點出現 **HR 1.11（0.56–2.18）** 的「反向」點估計（finerenone 21/491 vs placebo 19/468） [baseline_goals_absolute_Neves_2026]。但這是因為該亞群僅 7%、事件極少、CI 極寬；改用**絕對**風險差異檢定時**無異質性（P_interaction=0.13）** [baseline_goals_absolute_Neves_2026]。門診／講者切勿把這個點估計解讀為「控制好的人用 finerenone 傷腎」。

---

## 4. 合併用藥脈絡：GLP-1RA / SGLT2i 背景不改變 finerenone 的白蛋白尿效益

### 4.1 白話 🟡

第二個常見疑問：「病人已經在用 GLP-1RA（或要三合一），再加 finerenone＋SGLT2i 還有意義嗎？會不會疊高血鉀？」CONFIDENCE 的 GLP-1RA 次分析（Agarwal 2025，prespecified，**N=800，182 人（23%）基線用 GLP-1RA**）回答：**有意義，且不疊高血鉀** [baseline_goals_absolute_Agarwal_2025]。

### 4.2 數字 🟡（代理終點：UACR）

- **day 180 UACR 降幅在有/無 GLP-1RA 者一致**：合併治療 **−51%（−59 to −40）有 GLP-1RA vs −56%（−62 to −50）無 GLP-1RA**；finerenone 單用 −34% vs −37%；empagliflozin 單用 −36% vs −33% [baseline_goals_absolute_Agarwal_2025]。
- **各門檻交互作用皆不顯著**：>30% 降幅 P_interaction=0.60、>40% =0.79、>50% =0.84 [baseline_goals_absolute_Agarwal_2025]。
- **高血鉀不因加 GLP-1RA 而升高**：合併治療組 treatment-emergent 高血鉀 **9.0%（有 GLP-1RA）vs 9.5%（無 GLP-1RA）** [baseline_goals_absolute_Agarwal_2025]。

### 4.3 CONFIDENCE 主結果（同步起始 finerenone＋empagliflozin）🟡

主試驗（Agarwal 2025 NEJM）：合併治療 day 180 UACR **比單用 finerenone 多降 29%（LS mean ratio 0.71，0.61–0.82；P<0.001）、比單用 empagliflozin 多降 32%（0.68，0.59–0.79；P<0.001）**；**合併組較基線降 52%**（與 finerenone 單用 32%＋empagliflozin 單用 29% 的完全可加預期一致） [r2_Agarwal_2025]。高血鉀（investigator-reported）合併組 25（9.3%）vs finerenone 30（11.4%）vs empagliflozin 10（3.8%）——**加 SGLT2i 使高血鉀相對低約 15–20%** [r2_Agarwal_2025]。

> **證據性質誠實**：CONFIDENCE 為 **UACR 替代終點、180 天短期試驗，尚無硬終點**；講者宜明確標示其地位。「finerenone＋RASi＋SGLT2i 三劑」與「再加 GLP-1RA」的**硬終點**協同效益仍待專門研究 [baseline_goals_absolute_Agarwal_2025]。

---

## 5. 胰島素阻抗：機轉假說，證據極弱（abstract-only）📌🔴

Zhao 2026（單中心回溯、**n=45**、12 個月，status: abstract_only）以 HOMA-IR／TyG 指數觀察 finerenone 是否改善胰島素阻抗：HOMA-IR 中位 34.40→25.22→19.44（P=0.038）、TyG 9.49→9.04→8.93（P<0.007），並列 UACR、eGFR 變化 [baseline_goals_absolute_Zhao_2026]。**此為單臂、無對照、小樣本的機轉假說探索，且僅 abstract 可稽核——不足以支持任何臨床斷言，本檔不擴張其數字，僅列為未來研究方向。**

---

## 📊 簡報數據參考（從原文圖／表擷取）

> 以下數字皆逐字擷取自本地全文 MD，供直接貼入投影片；末欄標「來源檔 : grep 行號」。abstract-only 檔（Zhao_2026、Zuin_2026）僅取其 abstract 內明列值，不外推。

### 表 A — HF 結局（FIGARO-DKD，無 vs 有 HF 病史）

| 結局 / 族群 | Finerenone n（%）／事件率 | Placebo n（%）／事件率 | HR / rate ratio (95% CI) | ARR₄₈ / NNT | 來源 : 行號 |
|---|---|---|---|---|---|
| 新發 HF（無 HF 病史者首次 HHF） | 65/3396 (1.9%)；0.57/100py | 95/3385 (2.8%)；0.84/100py | HR 0.68 (0.50–0.93)；P=0.016 | ARR 1.1%；NNT 91 (49–605) | Filippatos_2022 : 59–60 |
| CV 死亡或首次 HHF | 290/3686 (7.9%) | 351/3666 (9.6%) | HR 0.82 (0.70–0.95)；P=0.011 | ARR 1.8%；NNT 55 (29–393) | Filippatos_2022 : 64 |
| HF 死亡或首次 HHF | 120/3686 (3.3%) | 173/3666 (4.7%) | HR 0.68 (0.54–0.86)；P=0.0013 | ARR 1.7%；NNT 60 (35–177) | Filippatos_2022 : 65 |
| 首次 HHF | 117/3686 (3.2%) | 163/3666 (4.4%) | HR 0.71 (0.56–0.90)；P=0.0043 | ARR 1.4%；NNT 70 (39–292) | Filippatos_2022 : 66 |
| 總 HHF（首次＋復發） | — | — | rate ratio 0.70 (0.52–0.94) | 累積事件 −3.0% | Filippatos_2022 : 69 |
| CV 死亡或首次 HHF（**有** HF 病史） | 54/290 (18.6%) | — | P_interaction=0.81 | ARR₄₈ **−4.8%** (−13.7–4.1) | Filippatos_2022 : 72, 76 |
| CV 死亡或首次 HHF（**無** HF 病史） | 236/3396 (6.7%) | — | （同上，不被病史修飾） | ARR₄₈ **−1.6%** (−3.1–0.0) | Filippatos_2022 : 72, 76 |

### 表 B — 有 HF 病史者統合分析（Jaiswal，2 RCT，n=1,007）

| 結局 | 效應量 (95% CI) | P / I² | 來源 : 行號 |
|---|---|---|---|
| 首次 HHF | OR 0.68 (0.47–0.98) | P=0.04；I²=0% | Jaiswal_2024 : 52 |
| 心血管複合 | OR 0.79 (0.60–1.04) | 非顯著；I²=0% | Jaiswal_2024 : 53 |
| 高血鉀 | OR 2.16 (1.38–3.38) | P<0.001；I²=0% | Jaiswal_2024 : 54 |

### 表 C — LVH 分層（FIDELITY，森林圖 Figure 1，LVH 盛行 9.6%）

| 結局 | LVH HR (95% CI) | 無 LVH HR (95% CI) | P_interaction | 來源 : 行號 |
|---|---|---|---|---|
| 整體 CV 複合 | 0.72 (0.55–0.95) | 0.89 (0.81–0.98) | 0.1075（NS） | Filippatos_2024 : 54, 57 |
| 整體腎臟複合 | 0.56 (0.38–0.84) | 0.80 (0.69–0.93) | 0.1782（NS） | Filippatos_2024 : 55, 57 |
| **HHF** | **0.34 (0.19–0.61)** | 0.86 (0.72–1.03) | **0.0024（顯著）** | Filippatos_2024 : 60 |
| TE 高血鉀 | 12.3% vs 5.7%（安慰劑） | 14.2% vs 7.0% | 停藥 1.5% vs 1.7% | Filippatos_2024 : 64 |

### 表 D — 基線治療目標達標度（Neves，FIDELITY，N=12,990）

| 項目 | 0 目標 | 1 目標 | 2 目標 | ≥3 目標 | 整體 | 來源 : 行號 |
|---|---|---|---|---|---|---|
| 佔比（n） | 29% (3732) | 40% (5208) | 24% (3091) | 7% (959) | — | Neves_2026 : 73 |
| 安慰劑 CV 事件率/100py | 6.0 | 5.1 | 4.3 | 3.5 | — | Neves_2026 : 105 |
| CV 複合 HR (95% CI) | 0.90 (0.76–1.05) | 0.79 (0.68–0.92) | 0.88 (0.72–1.08) | 0.89 (0.59–1.37) | 0.86 (0.78–0.95)；P_int 0.7481 | Neves_2026 : 116–119 |
| 腎臟複合 HR (95% CI) | 0.77 (0.60–0.97) | 0.71 (0.57–0.88) | 0.70 (0.50–0.97) | **1.11 (0.56–2.18)** | 0.76 (0.66–0.88)；P_int 0.6095 | Neves_2026 : 129–133 |
| HHF HR（P_int 0.7288） | 0.73 (0.54–0.99) | 0.84 (0.65–1.09) | 0.74 (0.53–1.04) | 0.49 (0.23–1.03) | 0.78 (0.66–0.92) | Neves_2026 : 122–123 |
| 全因死亡（整體） | — | — | — | — | 0.89 (0.79–1.00)；P_int 0.0659 | Neves_2026 : 139 |

> 註：≥3 目標腎臟 HR 1.11 為少事件、寬 CI 之點估計；絕對風險差異檢定無異質性（P_interaction=0.13） [baseline_goals_absolute_Neves_2026 : 134]。

### 表 E — 合併用藥脈絡（CONFIDENCE，代理終點 UACR，day 180）

| 分析 / 分層 | 效應量 (95% CI) | P_interaction / 安全 | 來源 : 行號 |
|---|---|---|---|
| 合併治療 UACR，有 GLP-1RA (n=182) | −51% (−59 to −40) | — | Agarwal_2025(GLP) : 45, 127 |
| 合併治療 UACR，無 GLP-1RA | −56% (−62 to −50) | — | Agarwal_2025(GLP) : 45, 127 |
| >30% / >40% / >50% 門檻 | — | P_int 0.60 / 0.79 / 0.84 | Agarwal_2025(GLP) : 143, 153, 163 |
| 合併治療高血鉀（GLP+ vs GLP−） | 9.0% vs 9.5% | 相近 | Agarwal_2025(GLP) : 179 |
| 合併 vs finerenone 單用（UACR） | ratio 0.71 (0.61–0.82)；多降 29% | P<0.001 | r2_Agarwal_2025 : 34, 107 |
| 合併 vs empagliflozin 單用（UACR） | ratio 0.68 (0.59–0.79)；多降 32% | P<0.001 | r2_Agarwal_2025 : 34, 107 |
| 合併治療 UACR 較基線 | −52% | 完全可加（32%＋29%） | r2_Agarwal_2025 : 309 |
| 高血鉀（investigator-reported） | 合併 9.3% / fine 11.4% / empa 3.8% | 加 SGLT2i 低約 15–20% | r2_Agarwal_2025 : 279, 328 |

### 表 F — abstract-only（不擴張）📌

| 主題 / 檔 | 可稽核值（僅 abstract） | 來源 : 行號 |
|---|---|---|
| 胰島素阻抗（Zhao，n=45，單臂） | HOMA-IR 34.40→25.22→19.44 (P=0.038)；TyG 9.49→9.04→8.93 (P<0.007) | Zhao_2026 : 65–66 |
| Fragility（Zuin，FIDELITY HHF） | HR 0.78、NNT 91、FI 23（HHF 最 robust） | Zuin_2026 : 43, 60 |

---

## 誠實邊界（Evidence limits）🟡🔴

- FIGARO HF 分析（Filippatos 2022）為 **prespecified**，等級較高，但仍為單一試驗次分析、HF 病史由 investigator 認定、無 LVEF／利鈉肽界定 🟡。
- LVH 分析（Filippatos 2024）為 **post hoc、ECG 無中央裁決、缺 echo**，HHF 的顯著交互屬 **hypothesis-generating**，不應據此篩選病人 🔴。
- Neves 2026 明言此達標度分析**非 prespecified、屬 exploratory**、隨機化未依達標數分層；≥3 目標亞群僅 7%、事件少 🟡。
- CONFIDENCE（含 GLP-1RA 次分析）為 **UACR 替代終點、180 天短期**，無硬終點；GLP-1RA 使用**未隨機化**，因果交互未檢定 🟡🔴。
- Zhao 2026（胰島素阻抗）、Zuin 2026（fragility）皆 **status: abstract_only**，僅 abstract 可稽核，本檔不擴張其數字 🔴。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|------|------|------------------|
| 無 HF 病史者仍能防新發 HF（HR 0.68，NNT 91） | 🟡 prespecified | `hf_kidney_spectrum_Filippatos_2022` 📄 |
| 有 HF 病史者絕對受益約 3 倍（ARR −4.8% vs −1.6%） | 🟡 prespecified | `hf_kidney_spectrum_Filippatos_2022` 📄 |
| 有 HF 病史統合：首次 HHF OR 0.68、高血鉀 OR 2.16 | 🟡 meta | `hf_kidney_spectrum_Jaiswal_2024` 📄 |
| LVH 對 HHF 顯著交互（HR 0.34，P_int 0.0024） | 🔴 post hoc / hypothesis | `hf_kidney_spectrum_Filippatos_2024` 📄 |
| 達標愈多絕對風險愈低，但療效不因達標改變 | 🟡 exploratory | `baseline_goals_absolute_Neves_2026` 📄 |
| GLP-1RA 背景不改變 UACR 效益與高血鉀 | 🟡 prespecified，代理終點 | `baseline_goals_absolute_Agarwal_2025` 📄 |
| 合併 finerenone＋empagliflozin UACR −52%（可加） | 🟡 代理終點，180 天 | `r2_Agarwal_2025` 📄 |
| finerenone 改善胰島素阻抗 | 🔴 abstract-only，n=45 單臂 | `baseline_goals_absolute_Zhao_2026` 📌 |
| HHF 為最 robust 之 CV 獲益（fragility） | 🔴 abstract-only | `baseline_goals_absolute_Zuin_2026` 📌 |

## 本地全文語料（可 grep 稽核）

📄 全文：`hf_kidney_spectrum_Filippatos_2022`（FIGARO HF 分析）、`hf_kidney_spectrum_Filippatos_2024`（FIDELITY LVH 短通訊）、`hf_kidney_spectrum_Jaiswal_2024`（有 HF 病史統合）、`baseline_goals_absolute_Neves_2026`（FIDELITY 治療目標達標度）、`baseline_goals_absolute_Agarwal_2025`（CONFIDENCE GLP-1RA 次分析）、`r2_Agarwal_2025`（CONFIDENCE 主結果 NEJM）。
📌 僅 abstract：`baseline_goals_absolute_Zhao_2026`（胰島素阻抗，n=45）、`baseline_goals_absolute_Zuin_2026`（fragility 分析）。

---

## References（本地可稽核）

1. Filippatos G, Anker SD, Agarwal R, et al. Finerenone Reduces Risk of Incident Heart Failure in Patients With CKD and Type 2 Diabetes: Analyses From the FIGARO-DKD Trial. *Circulation.* 2022;145:437-447. 📄 [hf_kidney_spectrum_Filippatos_2022]
2. Filippatos G, Anker SD, Bakris GL, et al. Finerenone and left ventricular hypertrophy in chronic kidney disease and type 2 diabetes. *ESC Heart Fail.* 2025;12:185-188. 📄 [hf_kidney_spectrum_Filippatos_2024]
3. Jaiswal V, Latif F, Naz S, et al. Efficacy of finerenone in reducing heart failure outcomes in patients with history of heart failure: A meta-analysis of RCTs. *IJC Heart Vasc.* 2024;55:101548. 📄 [hf_kidney_spectrum_Jaiswal_2024]
4. Neves JS, Leite AR, Vasques-Nóvoa F, et al. Outcomes With Finerenone by Baseline Treatment Goals in Type 2 Diabetes and CKD: A FIDELITY Analysis. *Diabetes Obes Metab.* 2026;28(7):6022-6033. 📄 [baseline_goals_absolute_Neves_2026]
5. Agarwal R, et al. Impact of Baseline GLP-1 RA Use on Albuminuria Reduction and Safety With Simultaneous Initiation of Finerenone and Empagliflozin (CONFIDENCE Trial). 2025. 📄 [baseline_goals_absolute_Agarwal_2025]
6. Agarwal R, Green JB, Heerspink HJL, et al. Finerenone plus Empagliflozin in Chronic Kidney Disease and Type 2 Diabetes (CONFIDENCE). *N Engl J Med.* 2025. 📄 [r2_Agarwal_2025]
7. Zhao X, Liu B, Sun R, et al. Associations of finerenone with reduced insulin resistance in patients with T2D and CKD: a real-world observational study. *J Diabetes Investig.* 2026. 📌 abstract-only [baseline_goals_absolute_Zhao_2026]
8. Zuin M, Bilato C, Temporelli PL, et al. Fragility analysis of cardiovascular outcomes with finerenone in T2DM and CKD. *Eur J Heart Fail.* 2026. 📌 abstract-only [baseline_goals_absolute_Zuin_2026]

---
*此檔為主題四叢集三之延伸拆解＋簡報數據集，撰寫日期基準 2026-07-11。所有具體數字均可 grep 回上列本地全文 MD（abstract-only 檔僅取 abstract 內明列值）。LVH 對 HHF 之顯著交互屬 post hoc／hypothesis-generating；治療目標達標度分析屬 exploratory；CONFIDENCE 為 UACR 替代終點短期試驗——以上均明示於誠實邊界，不作硬終點宣稱。*
