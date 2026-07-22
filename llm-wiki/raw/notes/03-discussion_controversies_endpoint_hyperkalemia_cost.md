# Discussion · 三大爭議：UACR 主終點、短期高血鉀、費用與依從性

> 本檔為主題三（第四支柱還是提早聯用？）主文 §4「Discussion：三大爭議」之延伸拆解，把該節（骨幹）獨立擴充成學術完整版：完整交代 CONFIDENCE 的研究設計，對每個關鍵結果給效應量＋CI＋P，並嚴格區分 primary／secondary／exploratory／surrogate／editorial 意見，明示每個論斷的證據邊界。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（不對其未載內容作具體數字斷言）。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織與改寫，所有作者／年份／數字均出自本地 MD 檔。
>
> **證據分層**：🟢 guideline routine（已進指引常規）｜🟡 evidence expansion（surrogate／post hoc／次分析／統合／模型）｜🔴 hypothesis（尚待專屬 RCT 驗證，或屬未定稿草案／editorial 意見）。
>
> **交叉連結（勿重複內容）**：統計迷思與臨床轉換見同資料夾 [`statistical_insights_myths.md`](statistical_insights_myths.md)；本檔上游脈絡見主文 [`03_fourth_pillar_or_early_combination.md`](03_fourth_pillar_or_early_combination.md) §4。

---

## 0. 一句話定位

CONFIDENCE 是第一個**隨機化**直接檢驗「finerenone＋SGLT2i 同步起始」的試驗，但它同時是三大爭議的引信：**(1) 主終點是 UACR 這個 surrogate，不是硬腎終點；(2) 同步起始並未在短期抵消 finerenone 介導的高血鉀；(3) 多支柱同步起始的費用、pill burden 與真實世界依從性未被試驗回答**。本檔把這三點各自拆成「可稽核的數字＋誠實的證據邊界」，讓後續引用時能精準區分「RCT surrogate 已證實」「統合分析方向性」「機轉假說」三個層級。

---

## 1. 三大爭議的共同底盤：CONFIDENCE 的研究設計（先交代，才好評斷）🟡

要評斷三大爭議，必須先把被爭議的那個試驗講清楚。CONFIDENCE（NCT05254002）為**隨機、雙盲、double-dummy、三臂平行的 Phase 2** 試驗，將已在最大耐受 RASi 背景下的 T2D＋albuminuric CKD 患者以 **1:1:1** 隨機分入 empagliflozin 單藥、finerenone 單藥、或兩者合併，治療 **180 天** [confidence_trial_Agarwal_2026]。納入 eGFR 30–90 mL/min/1.73 m²、UACR 100–5000 mg/g（Part A 原為 eGFR 40–90、UACR 300–5000，經 DMC 確認安全後於協定修訂放寬）[confidence_trial_Vaduganathan_2025]。finerenone 於 eGFR ≥60 起始 20 mg/d、eGFR <60 起始 10 mg/d；empagliflozin 10 mg/d；隨機化依 **eGFR（<60 vs ≥60）與 UACR（≤850 vs >850）** 分層 [confidence_trial_Agarwal_2026]。**關鍵排除**：screening 血鉀 >4.8 mmol/L、T1D、有症狀 HFrEF、90 天內心血管事件、以及 8 週內曾用 SGLT2i 或鉀結合劑 [confidence_trial_Agarwal_2026]。

**終點層級（爭議一的根源就在這裡）**：**primary** = 自 baseline 到 Day 180 的 UACR 相對變化；**secondary** = Day 180 UACR 下降 >30% 的比例（ADA 建議之治療優化門檻）；安全性系統性收集 hyperkalemia、AKI、30±4 天 >30% eGFR 下降、症狀性低血壓等 [confidence_trial_Vaduganathan_2025]。**試驗僅 180 天、且刻意設計為 surrogate 試驗**——這既是它能快速回答「同步安不安全、UACR 有無加成」的優點，也是三大爭議的共同來源。

---

## 2. 爭議一：主終點是 UACR，不是 hard renal outcome

### 2.1 正方（Georgianos／Cheng）：surrogate 有堅實的中介學基礎 🟡

正方的核心論證是「硬終點 RCT 在現實上不可行，而 UACR 是被驗證過的 mediator」。Georgianos 明算：一個為偵測硬腎終點（kidney failure、doubling creatinine、renal death 複合）差異而 power 的 Phase 3 試驗，估計需隨機化**約 41,000 人**，可預見的未來不會有這種 outcome trial [combination_editorial_Georgianos_2025]。而早期 albuminuria 下降正是 SGLT2i 與 finerenone 長期硬腎益處的**主要中介**：2019 年的 patient-level 統合（**41 個試驗、29,979 人**，3935 人達複合腎終點、中位追蹤 **3.4 年**）顯示，前 6 個月 **≥30% albuminuria 下降對應長期複合腎終點風險降 27%（HR 0.73；95% CI 0.67–0.81）**，且在高／極高基線 albuminuria 者更強 [combination_editorial_Georgianos_2025]。

CONFIDENCE 的 primary 結果落在這條中介曲線的「有利端」：Day 180 combination 使 UACR 自基線降約 **52%**，對比 finerenone 單藥 **32%**、empagliflozin 單藥 **29%**；組間 combination 較 finerenone 多降 **29%（LS mean ratio 0.71；95% CI 0.61–0.82；P<0.001）**、較 empagliflozin 多降 **32%（LS mean ratio 0.68；95% CI 0.59–0.79；P<0.001）** [combination_editorial_Cheng_2025][combination_editorial_Georgianos_2025]。而其 **secondary** 終點（>30% UACR 下降）在各 KDIGO 風險層皆過半（low/moderate 58.1%、high 74.2%、very high 70.6%），恰跨過上述中介學的門檻 [confidence_trial_Vaduganathan_2025]。Georgianos 因此直言「改變日常臨床實務的時機就是現在」；Cheng 則整合進「pillar risk-based」框架，主張以 KDIGO heatmap 導引、對高風險者同步或快速序列起始以打破 therapeutic inertia [combination_editorial_Georgianos_2025][combination_editorial_Cheng_2025]。

### 2.2 保留方（Wen 統合）：相對 SGLT2i 單藥，硬終點 additivity 未證實 🟡

保留方把尺度拉到「硬終點、且以正確的比較臂」。Wen 的系統性回顧與統合分析（隨機與觀察研究併入、random-effects）給出兩組方向相反的訊號 [hyperkalemia_combo_Wen_2026]：

- **相對 finerenone 單藥**，combination 顯著較優：all-cause mortality **OR 0.58（95% CI 0.36–0.93）**、MACE **OR 0.70（0.51–0.97）**、MAKE **OR 0.63（0.44–0.89）**。
- **相對 SGLT2i 單藥**，combination **無顯著額外益處**：mortality **OR 0.73（0.47–1.13；p=0.16）**、MACE **OR 0.77（0.55–1.08；p=0.14）**、MAKE **OR 0.87（0.58–1.31；p=0.51）**，且複合腎終點亦無顯著加成。

Wen 的 **trial sequential analysis（TSA）** 進一步指出：mortality、MACE、MAKE 的累積 Z 曲線**尚未跨越 monitoring boundary、也未進入 futility zone**，故硬終點的 additivity「仍需足夠 power 的 RCT」；作者對 mortality 與 UACR 給 moderate certainty、對 MACE／MAKE 僅 low certainty，並提示部分終點有 publication bias 之虞 [hyperkalemia_combo_Wen_2026]。

### 2.3 爭議一小結表

| 面向 | 正方（Georgianos/Cheng） | 保留方（Wen） |
|---|---|---|
| 終點性質 | UACR 為受驗證之 surrogate（27% 中介、HR 0.73） | UACR 終究非硬終點；硬終點 additivity 未證 |
| 對照臂 | vs 任一單藥皆 UACR 加成（LSMR 0.71／0.68） | vs SGLT2i 單藥 mortality/MACE/MAKE 皆 NS |
| 統計裁決 | 硬終點 RCT 需 ~41,000 人、不可行 | TSA：Z 曲線未越界，尚需 RCT |
| 引用邊界 | 可講「UACR over-additive」🟡 | 不可講「combination 降低硬終點」🔴 |

> **誠實邊界**：本爭議雙方其實不矛盾——「同步起始使 UACR over-additive」是 **RCT surrogate 已證實** 🟡；「同步起始降低硬終點」目前**無專屬 RCT、且相對 SGLT2i 單藥未達顯著** 🔴。引用時務必標明比較臂與終點層級。

---

## 3. 爭議二：SGLT2i 未能在短期抵消 finerenone 的高血鉀（本主題最反直覺者）

### 3.1 CONFIDENCE 的隨機化裁決：同步起始「不抵消」高血鉀 🟡

臨床上最誘人的假說是「SGLT2i 的 kaliuresis 能中和 finerenone 的高血鉀」。CONFIDENCE 的**預設高血鉀次分析**（JACC，本地全文 📄）用隨機化證據直接否證了「同步起始能抵消」這一版本 [confidence_trial_Agarwal_2026]：

- 高血鉀（K >5.5 mmol/L）整體發生於 **113/779（14.5%）**：combination **40/265（15.1%）**、finerenone **48/255（18.8%）**、empagliflozin **25/259（9.7%）** [confidence_trial_Agarwal_2026]。（Cheng editorial 以另一分母報 **15.3% vs 18.6%**，方向一致 [combination_editorial_Cheng_2025]。）
- **combination 與 finerenone 之間**：血鉀平均變化**無顯著差異（P=0.91）**、發生高血鉀之 odds **無顯著差異（P=0.85）**——即同步加上 SGLT2i **並未**顯著減少 MRA 介導的高血鉀 [confidence_trial_Agarwal_2026]。
- 以 empagliflozin 單藥為參照的 adjusted OR：combination **2.69（95% CI 1.46–4.96）**、finerenone **2.56（95% CI 1.42–4.59）**——兩個含 finerenone 的臂風險相近、且都高於單用 SGLT2i [confidence_trial_Agarwal_2026]。
- 高血鉀的**決定因子**為基線血鉀（aOR **9.23**／每升高 1 mmol/L；95% CI 5.07–16.81）與低 eGFR（aOR **1.11**／每降 5 mL/min/1.73 m²；95% CI 1.03–1.20），與時序無關 [confidence_trial_Agarwal_2026]。

**因果面（消除另一種行銷話術）**：causal mediation 分析顯示，比較 finerenone 與 combination 時，高血鉀對 UACR 下降的 percent mediation 僅 **0.2%**——**高血鉀不在 UACR 下降的因果路徑上**，且療效「regardless of development of hyperkalemia」皆維持 [confidence_trial_Agarwal_2026]。這既拿掉「療效靠升鉀」的疑慮，也拿掉「同步 SGLT2i 讓 finerenone 更安全」的短期證據。

### 3.2 把兩種對照拆開：相對誰而言「高血鉀更高」？🟡

Wen 統合把「相對誰」講清楚，避免混為一談 [hyperkalemia_combo_Wen_2026]：

- **相對 finerenone 單藥**：combination 高血鉀**無顯著差異（OR 1.09；95% CI 0.52–2.28）**——加 SGLT2i 沒放大 finerenone 的高血鉀（但也沒消除）。
- **相對 SGLT2i 單藥**：combination 高血鉀**顯著較高（OR 3.00；95% CI 2.50–3.61）**——因為你多加了一個升鉀藥。

### 3.3 Sinclair／Edmonston 的「時序假說」：同步 vs 序列，可能是關鍵 🔴

editorial（Sinclair & Edmonston，本地全文 📄）提出**時序假說**來調和 CONFIDENCE 與慢性/觀察資料的矛盾。在 FIVE-STAR 次分析中，finerenone 使 UACR 較安慰劑多降 **29%**（24 週、不受背景治療影響）；血鉀整體升 **0.22 mEq/L**，但**依基線是否已用 SGLT2i 分歧**——未用者升 **0.37 mEq/L**、已用者僅升 **0.13 mEq/L（P for interaction = 0.02）** [hyperkalemia_combo_Sinclair_2026]。機轉推測為 SGLT2i 需時間誘導遠端小管鉀處理的適應（動物模型中 dapagliflozin 保留近端 **Kcnk1**〔TWIK-related K channel 1〕表現）；**同步起始時，finerenone 的升鉀在 SGLT2i 尚未「適應」前就發生，故無法被抵消**；序列（SGLT2i 先行）則讓適應先建立 [hyperkalemia_combo_Sinclair_2026]。

Sinclair 因此呼籲一個**直接的三臂 sequencing RCT**（finerenone-first／同步／SGLT2i-first，以血鉀變化為主要終點，次要含 incident K >5.5、>6.0、治療中斷、成功 rechallenge、achieved finerenone dose、albuminuria）[hyperkalemia_combo_Sinclair_2026]。

> **證據邊界（極重要）**：FIVE-STAR 的 SGLT2i 使用**未隨機化**、存在 confounding by indication、子組樣本小且未校正多重比較；作者明示此為 **hypothesis-generating** 🔴。故臨床啟示只能講到：「若首要顧慮是血鉀，SGLT2i 先行在機轉上**可能**較同步起始安全——但待專屬 RCT 驗證」，**不可**當已確立事實。同步起始不抵消高血鉀，才是目前唯一的隨機化結論（CONFIDENCE）🟡。

### 3.4 爭議二小結表

| 比較 | 高血鉀結果 | 來源檔 |
|---|---|---|
| combination vs finerenone 單藥（隨機） | 血鉀變化 P=0.91、odds P=0.85（不抵消） | `confidence_trial_Agarwal_2026` 📄 |
| combination vs finerenone 單藥（統合） | OR 1.09（0.52–2.28）NS | `hyperkalemia_combo_Wen_2026` 📄 |
| combination vs SGLT2i 單藥（統合） | OR 3.00（2.50–3.61）顯著較高 | `hyperkalemia_combo_Wen_2026` 📄 |
| 高血鉀 → UACR 中介 | 0.2%，不在因果路徑 | `confidence_trial_Agarwal_2026` 📄 |
| 慢性 SGLT2i 背景再加 finerenone | K 僅升 0.13 vs 0.37（P-int 0.02，非隨機） | `hyperkalemia_combo_Sinclair_2026` 📄 |

---

## 4. 爭議三：費用、複方負擔與依從性

### 4.1 Cheng：pillar 策略的代價是「更高費用＋同時副作用」🟡

Cheng 的 narrative review 在倡議 pillar risk-based approach 之餘，明列其兩大代價：**更高的治療費用、以及同時起始多藥導致的同時副作用與 pill burden**（Fig. 3 逐字列 pillar 劣勢為「greater cost；simultaneous side effects」）[combination_editorial_Cheng_2025]。其務實解方是借鏡 HFrEF 的 GDMT 經驗——用**低劑量、多藥、快速序列**（如 STRONG-HF：N=1078，快速上調治療使再住院與死亡風險降低，**risk ratio 0.66；95% CI 0.50–0.86**），而非「一次全劑量全開」[combination_editorial_Cheng_2025]。

### 4.2 Agarwal & Fouque：真正的瓶頸是 education／adherence／access 🟡

Agarwal 與 Fouque 把費用問題放進「築牆」比喻：**築牆（疊加支柱）容易，但成本從第一到第四支柱遞增**，而 **education、adherence、access** 才是實踐的真正瓶頸 [r2_Agarwal_2023]。具體到 access：美國多數保險對「所有已被接受的支柱」仍需 **prior authorization**；不同國家藥價落差極大（印度 dapagliflozin 有學名藥、巴西由醫療體系免費提供）[r2_Agarwal_2023]。具體到 detection 缺口：在 **513,165 名** T2D 成人的 EHR 分析中，1 年期 UACR 與 eGFR 的中位檢測率僅 **51.6%**，且偵測到的高 albuminuria 盛行率隨 UACR 檢測率線性上升（檢測率 20%／50%／100% 對應盛行率 6%／15%／30%）——**大量 CKD＋T2D 病人根本未被診斷，遑論加藥** [r2_Agarwal_2023]。

### 4.3 CONFIDENCE 自身的 generalizability 限制 🟡

費用效益之爭也受限於試驗族群本身。Vaduganathan 明載 CONFIDENCE「had **stringent inclusion and exclusion criteria** that may limit the generalizability of findings to broader, more diverse populations, especially those at low risk」；且**治療僅 180 天**，長期（含心血管與腎臟硬終點）效果未評估、亦非為個別次組 power [confidence_trial_Vaduganathan_2025]。因此「同步起始對更廣、更低風險族群的成本效益」目前是**開放問題**，不能由 180 天 UACR 試驗外推。

> **這一爭議的誠實定位**：費用／pill burden／依從性屬 **editorial 意見與實作考量（🟡/🔴）**，本地語料**無**專屬的成本效益或真實世界依從性 RCT 可 grep。可講「pillar 策略代價明確、STRONG-HF 式快速序列或為折衷、access/adherence 是瓶頸」；**不可**宣稱「同步起始具成本效益」——那需要專屬研究。

---

## 5. 誠實邊界（Evidence limits）🟡🔴

- **CONFIDENCE 為 Phase 2、180 天、surrogate 試驗**：primary（UACR）為代理終點，硬腎/心血管終點未評估；stringent 納入限制外推 🟡 [confidence_trial_Vaduganathan_2025]。
- **爭議一**：「UACR over-additive」🟡 已由 RCT surrogate 證實；「降低硬終點」🔴 無專屬 RCT，且相對 SGLT2i 單藥 mortality/MACE/MAKE 皆 NS、TSA 未越界 [hyperkalemia_combo_Wen_2026]。
- **爭議二**：「同步起始不抵消高血鉀」🟡 為 CONFIDENCE 隨機化結論（P=0.91／0.85）；「SGLT2i 先行較安全」🔴 為時序假說，源自**非隨機**的 FIVE-STAR 次分析（confounding by indication、樣本小、未校正多重比較），僅 hypothesis-generating [confidence_trial_Agarwal_2026][hyperkalemia_combo_Sinclair_2026]。
- **爭議三**：費用／pill burden／依從性為 editorial 意見與流行病學 detection 資料（🟡/🔴）；本地無成本效益 RCT，「同步起始具成本效益」不可宣稱 [combination_editorial_Cheng_2025][r2_Agarwal_2023]。
- **Wen 統合**併入觀察性研究、部分終點僅 low certainty 且疑有 publication bias；OR 屬跨研究換算 🟡 [hyperkalemia_combo_Wen_2026]。
- 各數字專屬其原始族群（CONFIDENCE／FIVE-STAR／FIDELITY 統合／EHR 世代），外推須保留 🔴。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|---|---|---|
| UACR over-additive（52% vs 32%/29%；LSMR 0.71／0.68，P<0.001） | 🟡 RCT surrogate | `combination_editorial_Cheng_2025`、`confidence_trial_Vaduganathan_2025` 📄 |
| 早期 ≥30% albuminuria 降 → 硬腎終點降 27%（HR 0.73；41 試驗 29,979 人） | 🟡 中介學統合 | `combination_editorial_Georgianos_2025` 📄 |
| 硬終點 RCT 需 ~41,000 人、不可行 | 🟡 論證 | `combination_editorial_Georgianos_2025` 📄 |
| vs SGLT2i 單藥 mortality/MACE/MAKE 皆 NS；TSA 未越界 | 🔴 硬終點未證 | `hyperkalemia_combo_Wen_2026` 📄 |
| 同步起始不抵消高血鉀（P=0.91／0.85；14.5%，15.1/18.8/9.7%） | 🟡 RCT 隨機 | `confidence_trial_Agarwal_2026` 📄 |
| 高血鉀不在 UACR 因果路徑（mediation 0.2%） | 🟡 RCT 隨機 | `confidence_trial_Agarwal_2026` 📄 |
| combination vs finerenone OR 1.09；vs SGLT2i OR 3.00 | 🟡 統合 | `hyperkalemia_combo_Wen_2026` 📄 |
| SGLT2i 先行較同步降鉀（0.13 vs 0.37，P-int 0.02；Kcnk1） | 🔴 時序假說（非隨機） | `hyperkalemia_combo_Sinclair_2026` 📄 |
| pillar 代價＝費用＋同時副作用；STRONG-HF RR 0.66 | 🟡 editorial | `combination_editorial_Cheng_2025` 📄 |
| access/adherence 為瓶頸；prior auth；UACR 檢測率 51.6% | 🟡 editorial／流病 | `r2_Agarwal_2023` 📄 |
| CONFIDENCE 180 天、stringent、成本效益未答 | 🟡 限制 | `confidence_trial_Vaduganathan_2025` 📄 |
| 「同步起始降硬終點且具成本效益」之專屬 RCT | 🔴 尚無 | —（誠實揭露） |

## 本地全文語料（可 grep 稽核）

📄 全文：`confidence_trial_Agarwal_2026`（CONFIDENCE 高血鉀 JACC 次分析：設計／14.5%／P=0.91,0.85／mediation 0.2%）、`confidence_trial_Vaduganathan_2025`（KDIGO 風險分層次分析／設計／generalizability 限制）、`combination_editorial_Cheng_2025`（pillar risk-based／UACR 52/32/29／hyperkalemia 15.3/18.6／STRONG-HF）、`combination_editorial_Georgianos_2025`（41,000 人論證／29,979 人中介統合 HR 0.73／eGFR dip 6.3/3.8/1.1）、`hyperkalemia_combo_Wen_2026`（統合：vs 兩單藥之 mortality/MACE/MAKE/高血鉀 OR、TSA）、`hyperkalemia_combo_Sinclair_2026`（時序假說／FIVE-STAR 0.13 vs 0.37／sequencing RCT）、`r2_Agarwal_2023`（四支柱／費用遞增／access/adherence／513,165 EHR）。

---

## References（Vancouver 風格，含本地檔名）

1. Agarwal R, Green JB, Heerspink HJL, et al. Risk of hyperkalemia with empagliflozin, finerenone, or both: secondary analysis of the CONFIDENCE randomized trial. *J Am Coll Cardiol.* 2026;87(7):772–784. doi:10.1016/j.jacc.2025.10.049. 📄 [confidence_trial_Agarwal_2026]
2. Vaduganathan M, Green JB, Heerspink HJL, et al. Simultaneous initiation of finerenone and empagliflozin across the spectrum of kidney risk in the CONFIDENCE trial. *Nephrol Dial Transplant.* 2026;41(1):161–170. doi:10.1093/ndt/gfaf160. 📄 [confidence_trial_Vaduganathan_2025]
3. Georgianos PI, Koufakis T, Arampatzis S, Liakopoulos V. CONFIDENCE in the safety and efficacy of dual therapy with an SGLT-2 inhibitor and finerenone in patients with chronic kidney disease and type 2 diabetes. *Diabetes Obes Metab.* 2025;27(11):6097–6100. doi:10.1111/dom.70026. 📄 [combination_editorial_Georgianos_2025]
4. Cheng AYY, Mottl A, Magwire M. Pillar risk-based treatment for chronic kidney disease in people with type 2 diabetes: a narrative review. *Diabetes Ther.* 2025;16(11):2083–2099. doi:10.1007/s13300-025-01796-7. 📄 [combination_editorial_Cheng_2025]
5. Wen CF, Chuang MH, Wu VC, Chen JY. Efficacy of combined SGLT2 inhibitors and finerenone in chronic kidney disease: a systematic review and meta-analysis. *Front Pharmacol.* 2026;17:1803971. doi:10.3389/fphar.2026.1803971. 📄 [hyperkalemia_combo_Wen_2026]
6. Sinclair MR, Edmonston D. It's about time: potassium risk with combination guideline-directed medical therapy. *Kidney Int Rep.* 2026;11:106609. doi:10.1016/j.ekir.2026.106609. 📄 [hyperkalemia_combo_Sinclair_2026]
7. Agarwal R, Fouque D. The foundation and the four pillars of treatment for cardiorenal protection in people with chronic kidney disease and type 2 diabetes. *Nephrol Dial Transplant.* 2023;38(2):253–257. doi:10.1093/ndt/gfac331. 📄 [r2_Agarwal_2023]

---
*此檔為主題三之延伸拆解，撰寫日期基準 2026-07-12。所有具體數字均可 grep 回上列本地全文 MD。三大爭議的證據層級須嚴格區分：UACR over-additive 與「同步不抵消高血鉀」為 RCT surrogate/隨機結論（🟡）；「降硬終點」「SGLT2i 先行較安全」「同步具成本效益」皆屬未證實之假說或 editorial 意見（🔴），對應之專屬前瞻 RCT 目前不存在，為明示之研究缺口。*
