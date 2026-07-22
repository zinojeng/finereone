# 什麼『中介』了 finerenone 的心血管益處？——UACR 與 SBP 的因果中介分析與『未被捕捉的一半』

> 主題五的因果推論專論〈[血鉀是否中介 CV 益處](../05_hyperkalemia_egfr_dip_safety_engineering/potassium_mediation_of_cv_benefit.md)〉下了一個**否定判決**：血鉀（無論高低）**不**中介 finerenone 的心血管（CV）益處——正式中介分析中血鉀的中介比例僅 −1.5%（95% CI −38 to 7），落在 0 兩側。本檔接手那個判決留下的**正向問題**：既然血鉀不中介，那**到底是什麼在中介**？答案（來自同一份 Agarwal 2026 causal mediation）是：**UACR 與 SBP 兩條可測路徑合起來解釋約一半，另一半仍未被任何 biomarker 捕捉。** 本檔專講「什麼**部分**中介、以及為何**另一半仍未知**」，與 potassium 檔（什麼**不**中介）正向互補。
>
> 本檔**不重述** surrogate 驗證的方法學（trial-level R²、個體 vs 試驗層級、連續 vs 二元的統計陷阱），那些見同資料夾 [`statistical_insights_myths.md`](statistical_insights_myths.md)（迷思一至五）。本檔只做一件事：把「**mediation 比例**」這個量——效應被哪條可測路徑解釋了幾成——攤開來讀。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（不對其未載內容擴張，數字維持原樣）。每個具體數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。**LLM 僅負責組織、改寫與因果／統計詮釋；詮釋可延伸，數字一律 grep 回本地全文，不杜撰。**
>
> **證據分層**：🟢 已確立的因果推論／統計共識｜🟡 post hoc／causal mediation／模型推估｜🔴 假說、僅摘要（📌）或**尚未被任何 biomarker 量化**。

---

## ❓ 問題重述：中介分析在回答什麼？

Potassium 檔證明了「血鉀不是那條路」。但 finerenone 的 CV 益處是**真實存在**的（FIDELITY 5 年 total effect：relative mean survival 1.12，95% CI 1.04 to 1.21）[albuminuria_mediation_Agarwal_2026] 📄——它一定經由某些機轉傳遞。**Causal mediation analysis 的目的，就是把「這個效應被哪一條可測路徑解釋了幾成」這件事量化成一個百分比。**

Agarwal 2026 對 FIDELITY IPD（n=12,143）同時放進四個「月 4 biomarker 變化」當 mediator，檢定各自中介了多少 CV 複合益處（CV 死亡、非致死 MI、非致死中風、HHF；time-to-first）[albuminuria_mediation_Agarwal_2026] 📄。四個 biomarker 在月 4 **全都顯著改變**——UACR ↓32.2%、SBP ↓3.6 mmHg、體重 ↓0.23 kg、血鉀 ↑0.19 mEq/L[albuminuria_mediation_Agarwal_2026] 📄——但「**有沒有改變**」與「**有沒有中介**」是兩回事，這正是分析的價值所在。

> **淺白比喻「路徑分帳」**：finerenone 帶來的 CV 益處是一筆總帳（relative mean survival +12%）。中介分析像會計師把這筆帳拆進不同科目：有多少走「UACR 這條帳」、多少走「SBP 這條帳」、多少走「體重／血鉀」。**能記帳的前提是那條路可被測量**——UACR、SBP 是門診量得到的「可測的帳」；而抗發炎／抗纖維化的組織效應沒有對應的血檢科目，只能記進「**未列帳的雜項**」。本檔的核心發現，就是**可測的帳只湊出一半，另一半掛在未列帳的雜項裡。**

---

## 📊 UACR + SBP 的中介拆解：四個 mediator 的分帳表

以下是四個 mediator 各自與聯合的中介比例。**關鍵是把「改變幅度」與「中介比例」分開讀**——體重與血鉀都顯著改變了，卻不進帳。

| Mediator（月 4 變化，finerenone − placebo） | 顯著改變？ | 中介比例（含 A×M 交互） | 中介比例（不含交互） | 判定 |
|---|---|---|---|---|
| **UACR ↓32.2%**（95% CI −34.2 to −30.3） | 是 | **39%（7 to 71）** | **36%（7 to 64）** | ✅ 顯著中介（最大單一路徑） |
| **SBP ↓3.6 mmHg**（−4.1 to −3.1） | 是 | **21%（3 to 40）** | **22%（5 to 39）** | ✅ 顯著中介 |
| 體重 ↓0.23 kg（−0.32 to −0.13） | 是 | **4%（−1 to 9）** | — | ❌ 不顯著 |
| 血鉀 ↑0.19 mEq/L（0.17 to 0.20） | 是 | **−1.5%（−38 to 7）** | — | ❌ 不顯著（點估計為負） |
| **UACR + SBP 聯合** | — | **50%（21 to 100）** | **47%（26 to 100）** | ✅ 兩路徑合計約一半 |

（改變幅度見 [albuminuria_mediation_Agarwal_2026] 📄 摘要與 Table 2；中介比例見同檔 Results 與 Table 3。）

三個要讀懂的細節：

1. **UACR 是最大單一路徑，但只佔約四成。** UACR 中介 39%（含交互）／36%（不含），兩種模型一致——這與作者前作在同一資料集報告的「UACR 中介 37%」相符[albuminuria_mediation_Agarwal_2026] 📄。**UACR 是主要記帳科目，但遠非全部。**
2. **SBP 是第二條被證實的路徑。** SBP 中介 21%（含交互）／22%（不含）；作者指出這高於 Ruilope 以 time-varying SBP 估計的 12.6%，差異來自「mediator 測量時點與建模框架」不同[albuminuria_mediation_Agarwal_2026] 📄——同一條路徑、不同方法，比例就浮動，這本身是方法學保留（見下文 🔬）。
3. **聯合 ≠ 相加。** UACR 39% + SBP 21% = 60%，但聯合模型只有 50%——因為兩條路徑**部分重疊**（血流動力學與腎小球通透性有共同上游）。聯合模型扣掉重疊後，UACR 與 SBP「捕捉的是重疊但各自不同的機轉元素——分別是腎小球通透性與全身血流動力學」[albuminuria_mediation_Agarwal_2026] 📄。作者結論：兩者「共同解釋 finerenone 長期 CV 益處的**一半**（half）」[albuminuria_mediation_Agarwal_2026] 📄。

> **絕對尺度的錨**：這 50% 是掛在一筆不大的總帳上。UACR 路徑的 natural indirect effect 為 relative mean survival 1.04（1.02–1.06）[albuminuria_mediation_Agarwal_2026] 📄；總效應本身也只有 1.12。作者特別提醒：因為多數人在兩組都保持 event-free、事件率中等，**relative mean survival 才是更有意義的摘要，proportion-mediated 反而次要**[albuminuria_mediation_Agarwal_2026] 📄。所以「一半」是拆一筆溫和益處的帳，不是拆一個巨大效應。

---

## 🧩 未被捕捉的一半：可測的帳只湊出 50%

分帳表最重要的一格，其實是**表格外面**那一半。約 50% 的 CV 益處**不經** UACR／SBP／體重／血鉀任何一條可測路徑傳遞——作者明言「其餘一半並非由這些系統性標記所捕捉」（the remaining half ... not captured by these systemic markers）[albuminuria_mediation_Agarwal_2026] 📄。

這一半指向的是機轉層級、而非 biomarker 層級的東西：MR 阻斷對**心肌細胞、巨噬細胞、血管壁**的**直接抗纖維化與抗發炎效應**（direct antifibrotic and anti-inflammatory effects ... on cardiomyocytes, macrophages, and the vascular wall）[albuminuria_mediation_Agarwal_2026] 📄。作者把這歸因於 finerenone「對心肌 MR 的選擇性高親和力結合，產生獨立於全身血流動力學的抗纖維化與抗發炎效應」[albuminuria_mediation_Agarwal_2026] 📄。

**為什麼這一半「記不了帳」？** 不是因為它不存在，而是因為**沒有對應的臨床可測 biomarker**：組織纖維化、巨噬細胞浸潤這些效應，在 FIDELITY 裡沒有為全體病人量測發炎／纖維化標記（作者自陳 aldosterone、inflammatory/fibrosis markers 未在全體測量）[albuminuria_mediation_Agarwal_2026] 📄。**沒被測量的路徑，中介分析就記不進任何科目——它只能落進「未列帳的直接效應」。** 🔴 這一半目前**無任何單一 biomarker 能量化**，是機轉假說（antifibrotic/anti-inflammatory）而非已量化的中介路徑。

**排除法的雙面性**：這一半是「總效應 − 已記帳路徑」的**殘差**，用排除法推得。這既是它的說服力（體重、血鉀被正面排除，UACR/SBP 被正面證實，剩下的殘差不是「沒去驗」而是「驗過四條、湊不滿」），也是它的脆弱點（殘差可能混入模型設定誤差、mediator 測量誤差被低估的部分——見 🔬）。**誠實的說法是：「約一半未被這四個 biomarker 解釋」，而非「已證實一半來自抗纖維化」**；後者是機轉層級最合理的候選，但在本分析中沒有被任何量測直接證實。

> 這也回應了 potassium 檔的收斂判決：finerenone 益處的**主幹是組織層面的直接作用**——部分經 UACR/SBP「顯影」出來（可記帳的一半），另一半來自直接抗纖維化路徑（未列帳的一半）；血鉀既不在主幹、也不在任何一條記帳的支線上。

---

## ⏱️ 時序弔詭：CV 益處早於可測的腎保護

有一個時間軸上的弔詭，直接動搖「UACR 是唯一因果通道」的圖像：**CV 益處出現得比可測得的腎保護還早。**

- CV 益處「emerges within months, before measurable kidney protection」[albuminuria_mediation_Agarwal_2026] 📄；
- 而腎保護「requires approximately 18 months to become statistically apparent」[albuminuria_mediation_Agarwal_2026] 📄。

如果 UACR 降幅（腎保護的代理）是 CV 益處的**唯一**因果通道，那 CV 益處**不該早於**腎保護出現——時序對不上。這弔詭有兩層意涵：

1. **它支持「另一半來自快速的直接組織效應」**：CV 益處在腎保護可測之前就啟動，指向的是不需時間累積的即時血流動力學／抗發炎效應，而非慢慢兌現的腎結構保護[albuminuria_mediation_Agarwal_2026] 📄。
2. **它暴露「月 4 mediator → 後續事件」框架的時間錯配**：把「第 4 個月的一次 UACR 快照」當成解釋「後續數年事件」的中介，本身是一個方便的觀測窗，不是完整的因果時序。這也支持把 **UACR 理解成 finerenone 療效的「伴隨標記」（companion biomarker）而非唯一的因果閘門**——它與益處高度同行、可靠反映藥物在起作用，但益處並非全數「經過」它。（時序錯配的統計面詳見 [`statistical_insights_myths.md`](statistical_insights_myths.md) 迷思五。）

---

## 🔬 方法學保留：為什麼「一半」是點估計而非精確值

「50%」很好記，但它的可信賴度必須誠實標定。至少五重保留：

1. **CI 很寬，上界觸 100%。** 聯合中介 50%（95% CI 21 to 100）[albuminuria_mediation_Agarwal_2026] 📄——上界頂到 100% 意味精確度有限，「一半」是點估計、不是窄區間。單一路徑亦然：UACR 39%（7–71）、SBP 21%（3–40）。
2. **連續 vs 二元 mediator 給不同數字。** 本分析中 UACR 含交互 39%、不含交互 36%（差距小、算穩健）；但對照前作 Agarwal 2023：同一種效應，UACR 以**連續變項**中介 CV 37%、改用**二元（≥30% 門檻）**就掉到 26%（腎端更誇張：84% → 64%）[albuminuria_mediation_Agarwal_2023] 📌。**同一真實機轉不會因為你把 mediator 切成連續或門檻而改變——會變的是估計本身**，這正說明 point estimate 不宜當精確值讀。
3. **依賴不可檢驗的無殘餘混淆假設。** natural direct/indirect effect 的識別，前提是「mediator–outcome 之間無未測混淆」，這條假設「在目前 CMAverse 的存活結局實作中無法直接檢定」[albuminuria_mediation_Agarwal_2026] 📄。作者以 E-value 量化脆弱度：聯合 UACR+SBP 的 indirect effect E-value 僅 **1.29（近虛無端 1.19）**、UACR 1.25（1.14）、SBP 1.16（1.11）[albuminuria_mediation_Agarwal_2026] 📄——一個中等強度的未測混淆因子就可能把中介效應解釋掉。
4. **mediator 測量誤差會衰減中介比例。** UACR／SBP 本身測量變異大；測得越不準，估到的中介比例通常被**低估**。作者為此專跑敏感度分析（基線 SBP 假設 SD 2/4/6 mmHg、基線 UACR log 尺度 10%/20%/30%）[albuminuria_mediation_Agarwal_2026] 📄——真實中介或許比 50% 更高，但方向是「被低估」而非「被高估」。
5. **proportion-mediated 在某些次群會失去意義。** 當 treatment 與 mediator 效應方向相反時，這個指標「uninformative」，聯合中介在小次群中甚至「無法可靠估計」[albuminuria_mediation_Agarwal_2026] 📄。
6. **不易外推到其他藥。** 前作 Agarwal 2023 白紙黑字：「not readily extendable to other drugs」[albuminuria_mediation_Agarwal_2023] 📌。finerenone 的分帳結構專屬於 finerenone × FIDELITY 族群，不能搬給任何降 UACR 或降 SBP 的藥。

---

## 💡 臨床意涵：UACR 是腎益處的近完整指標、CV 益處的部分指標

把分帳結果翻成門診語言，三句話帶走：

- **早期 UACR 降幅是腎益處的近完整 surrogate、但只是 CV 益處的部分指標。** 前作 Agarwal 2023 顯示 UACR（連續）中介**腎**益處達 84%、但**CV**益處只有 37%[albuminuria_mediation_Agarwal_2023] 📌；本分析 UACR 中介 CV 39%[albuminuria_mediation_Agarwal_2026] 📄。**同一個 UACR，對腎幾乎全記帳、對 CV 只記了三、四成。**
- **門診用月 4 的 UACR 與 SBP 一起追療效反應是合理的**——作者主張兩者應作為「finerenone CV 療效的**互補**（complementary）臨床指標一起追蹤，而非互相競爭的 surrogate」[albuminuria_mediation_Agarwal_2026] 📄。UACR 反映腎小球通透性、SBP 反映全身血流動力學，兩條帳互補。
- **但不能只看 UACR 判斷 CV 益處，也不能把 UACR 無反應者當『無效』。** 因為 CV 益處有一半根本不經 UACR/SBP。UACR 沒大降的病人，其抗纖維化那一半益處可能照樣兌現——**UACR 無反應 ≠ CV 無獲益**。反過來也一樣，別把「UACR 漂亮」讀成「CV 已保住、可鬆手」。（呼應 `statistical_insights_myths.md` 迷思三：mediation % ≠ 機轉佔比。）
- **體重與血鉀不是療效 surrogate。** 兩者顯著改變卻不中介，作者直言是「poor surrogates」／「not useful surrogates for cardiovascular benefit」[albuminuria_mediation_Agarwal_2026] 📄——別把體重下降或血鉀變化讀成「藥在起作用」。

---

## 🔴 誠實邊界（Evidence limits）

- **Mediation ≠ 完整因果證明。** 50% 是「被兩條可測路徑統計解釋的比例」，不是「機轉的 50% 配額」；它依賴不可檢驗的無殘餘混淆假設（E-value 僅 1.29）[albuminuria_mediation_Agarwal_2026] 📄，屬 🟡 方法學保留。
- **未捕捉的一半無 biomarker 量化。** 抗纖維化／抗發炎的直接組織效應是 🔴 **機轉假說**，FIDELITY 未為全體測量發炎／纖維化標記[albuminuria_mediation_Agarwal_2026] 📄；「另一半」是被排除法推得的殘差，不是被正面量測到的路徑。
- **Agarwal 2023 為 abstract-only（📌）。** 其 84%／64%／37%／26%、median UACR 514、≥30% 降幅 53.2% vs 27.0% 均取自結構化摘要[albuminuria_mediation_Agarwal_2023] 📌，不對其未載內容擴張。
- **外推限制。** 具體分帳專屬 FIDELITY（T2D+CKD）。心衰場景（FINEARTS-HF，基線 median UACR 僅 17 mg/g）的 UACR 中介比例更低且 CI 更寬（複合 34%〔16–132〕、首次 HF 事件 29%〔14–82〕；二元化僅 15%／11%）[albuminuria_mediation_Mc_2025] 📌——但該檔亦為 abstract-only，僅供對照，不外推。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|---|---|---|
| UACR 中介 CV 益處 39%（含交互）／36%（不含），最大單一可測路徑 | 🟡 causal mediation | `albuminuria_mediation_Agarwal_2026` 📄 |
| SBP 中介 CV 益處 21%／22%，第二條被證實路徑 | 🟡 causal mediation | `albuminuria_mediation_Agarwal_2026` 📄 |
| UACR+SBP 聯合中介 50%（21–100），共同解釋「一半」 | 🟡 causal mediation | `albuminuria_mediation_Agarwal_2026` 📄 |
| 體重（4%）、血鉀（−1.5%）不中介、非有用 surrogate | 🟡 causal mediation | `albuminuria_mediation_Agarwal_2026` 📄 |
| **另一半未被捕捉**，指向直接抗纖維化／抗發炎組織效應 | 🔴 機轉假說（未量化） | `albuminuria_mediation_Agarwal_2026` 📄 |
| CV 益處早於可測腎保護（數月 vs ~18 月）之時序弔詭 | 🟡 | `albuminuria_mediation_Agarwal_2026` 📄 |
| 無殘餘混淆假設、E-value 1.29、測量誤差衰減、不易外推 | 🟡 方法學保留 | `albuminuria_mediation_Agarwal_2026` 📄 |
| 連續 vs 二元給不同% （UACR 84/64、CV 37/26）；不外推他藥 | 🔴 abstract-only | `albuminuria_mediation_Agarwal_2023` 📌 |
| HF 低白蛋白尿族群中介更低（34/29、15/11）—僅對照 | 🔴 abstract-only | `albuminuria_mediation_Mc_2025` 📌 |

---

## 本地全文語料（可 grep 稽核）

📄 全文：`albuminuria_mediation_Agarwal_2026`（四中介 causal mediation：n=12,143；月 4 變化 UACR −32.2%〔−34.2 to −30.3〕、SBP −3.6 mmHg、體重 −0.23 kg、血鉀 +0.19 mEq/L；UACR 中介 39%〔7–71〕含交互／36%〔7–64〕不含；SBP 21%〔3–40〕／22%〔5–39〕；體重 4%〔−1 to 9〕；血鉀 −1.5%〔−38 to 7〕；聯合 50%〔21–100〕／47%〔26–100〕；total effect relative mean survival 1.12〔1.04–1.21〕；UACR NIE 1.04〔1.02–1.06〕；E-value 聯合 1.29〔1.19〕、UACR 1.25〔1.14〕、SBP 1.16〔1.11〕；Ruilope SBP 12.6%、前作 UACR 37%；"emerges within months, before measurable kidney protection"、"approximately 18 months"、"remaining half ... not captured"、"antifibrotic and anti-inflammatory effects ... cardiomyocytes, macrophages, and the vascular wall"、"complementary indicators"、"not useful surrogates"、"uninformative"）。

📌 abstract（數字不擴張）：`albuminuria_mediation_Agarwal_2023`（FIDELIO+FIGARO；median UACR 514；≥30% 降幅 53.2% vs 27.0%；連續 kidney 84%／CV 37%；二元 kidney 64%／CV 26%；"not readily extendable to other drugs"）、`albuminuria_mediation_Mc_2025`（FINEARTS-HF；基線 median UACR 17；UACR 降 26% at 3 months；連續複合 34%〔16–132〕、首次 HF 29%〔14–82〕；二元 15%〔5–68〕／11%〔3–39〕）。

---

## References（Vancouver 風格，含本地檔）

1. Agarwal R, Filippatos G, Pitt B, et al. Systolic blood pressure and albuminuria reduction mediate cardiovascular benefits of finerenone in type 2 diabetes and CKD (causal mediation analysis of FIDELITY). Nephrol Dial Transplant. 2026. 📄 [albuminuria_mediation_Agarwal_2026]
2. Agarwal R, Tu W, Farjat AE, et al. Impact of finerenone-induced albuminuria reduction on chronic kidney disease outcomes in type 2 diabetes: a mediation analysis. Ann Intern Med. 2023;176(12):1606–16. 📌 abstract only [albuminuria_mediation_Agarwal_2023]
3. Mc Causland FR, Vaduganathan M, Claggett BL, et al. Changes in albuminuria and the effect of finerenone on cardiovascular outcomes: insights from FINEARTS-HF (abstract). Nephrol Dial Transplant. 2025;40(Suppl 3):gfaf116.0475. 📌 abstract only [albuminuria_mediation_Mc_2025]

---
*此檔為主題二〈從白蛋白尿到硬終點〉之因果中介專論，撰寫日期基準 2026-07-12。所有具體數字均可 grep 回上列本地全文 MD。核心論點：finerenone 的 CV 益處中，UACR（39%）與 SBP（21%）兩條可測路徑**聯合中介約一半（50%，95% CI 21–100）**，血鉀與體重不中介；**另一半不被任何系統性 biomarker 捕捉**，指向 MR 阻斷的直接抗纖維化／抗發炎組織效應（🔴 機轉假說、未量化）。時序弔詭（CV 益處早於可測腎保護）支持「UACR 是伴隨標記而非唯一因果閘門」。方法學保留：CI 寬（上界觸 100%）、連續 vs 二元不穩、依賴不可檢驗的無殘餘混淆假設（E-value 1.29）、不易外推。與 potassium 檔（什麼**不**中介）及 statistical_insights_myths 檔（surrogate 統計）互補，刻意不重複。Agarwal 2023／Mc 2025 為 abstract-only（📌），數字不擴張。*
</content>
</invoke>
