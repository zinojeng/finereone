# 低血鉀減少 54% 是否『中介』了 finerenone 的心血管益處？——關聯 vs 因果中介的判讀

> 本檔為主題五（高血鉀與 eGFR dip 的安全工程學）之**因果推論專論**，處理一個「百萬美元問題」：finerenone 把嚴重低血鉀（K<3.5）壓低了約一半（HR 0.46 ≈ 相對下降 54%），同時又降低心衰住院與心律不整（含猝死）；這兩條**平行下降的曲線**，是「共同上游各自產生」的**關聯**，還是「矯正低血鉀 → 減少猝死」的**因果中介（mediation）**？
>
> 本檔刻意**不重述**同資料夾兩檔的臨床描述——雙向電解質效應與 U 形風險見 [`hypokalemia_bidirectional_electrolyte.md`](hypokalemia_bidirectional_electrolyte.md)；「關聯≠因果」「time-updated」「非隨機暴露」等統計素養見 [`statistical_insights_myths.md`](statistical_insights_myths.md)（迷思三、四）。本檔只做一件它們沒做的事：**把「血鉀是否為中介變項」這個命題，放進正式的 causal mediation 框架裡判決**。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract。每個具體數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織、改寫與**因果詮釋**；詮釋可延伸，數字一律出自本地全文。
>
> **證據分層**：🟢 已確立的方法學／因果推論共識｜🟡 post hoc／次分析／代理終點／中介模型｜🔴 假說、僅摘要或**尚未被任何分析檢定**。

---


> 🔗 **正向互補**：血鉀**不**中介；那**什麼中介**（UACR 39%＋SBP 21%≈一半）見主題二 [`../02_albuminuria_to_hard_endpoints/uacr_sbp_mediation_of_cv_benefit.md`](../02_albuminuria_to_hard_endpoints/uacr_sbp_mediation_of_cv_benefit.md)。

## ❓ 問題重述：為什麼「平行下降」會讓人直覺想到因果中介？

先把兩條曲線並排擺出來——它們確實誘人：

- **電解質端**：FIDELITY 中 finerenone 把嚴重低血鉀（K<3.5）從 placebo 的 10.2%（650/6403）壓到 4.8%（309/6420），**HR 0.46（95% CI 0.40–0.53）**——相對下降約 54%（1−0.46）[label_guideline_safety_Pitt_2025]；FINEARTS-HF 得到**完全一致**的 K<3.5 **HR 0.46（95% CI 0.38–0.56）**[hf_renal_safety_Vardeny_2025]。
- **臨床端**：同一個 FIDELITY 族群，finerenone 把 CV 複合與心律不整複合分別降低 **14% 與 13%**（HHF 為主要驅動）[label_guideline_safety_Pitt_2025]；而 FIDELITY 的心律不整複合終點的**定義本身**就包含「new diagnosis of atrial fibrillation/atrial flutter, hospitalization due to arrhythmia, or **sudden cardiac death**」[label_guideline_safety_Pitt_2025]。

直覺的因果故事於是自動成形，而且**電生理上非常合理**：低血鉀會延長 QT、促發室性心律不整與猝死；既然 finerenone 矯正了低血鉀、又減少了含猝死的心律不整終點，「矯正低血鉀 → 減少猝死」看起來像是一條現成的因果鏈。連 Pitt 團隊自己都在論文裡把這個問題**明白地留成問號**：「it is not known if the reductions in these hazard outcomes with finerenone are **in part mediated by the prevention of hypokalaemia**; further investigation will be required」[label_guideline_safety_Pitt_2025]。

> **淺白比喻**：兩條曲線平行下降，有兩種完全不同的解釋。(a)**中介路徑**——「finerenone → 矯正低血鉀 → 減少猝死」，血鉀是**串在因果鏈中間的那一環**；(b)**共同上游**——「finerenone → MR 阻斷」這個上游**同時、但各自獨立地**生出兩個下游（血鉀被矯正 / 心臟被保護），兩個下游之間**沒有因果箭頭**。兩種情況畫出來的曲線長得一模一樣。**平行 ≠ 串聯。要分辨，只能做正式的中介分析。**

---

## 📊 平行關聯的證據（Pitt 2025 + Vardeny 2024）：兩個前提都成立，但都只是關聯

要讓「中介」假說成立，至少需要兩個前提，而現有資料**確實都支持**——這也是假說如此頑強的原因：

**前提一：低血鉀確實被 finerenone 矯正了。** 除上述 K<3.5 的 HR 0.46 外，中度低血鉀 K<4.0 也從 placebo 48.3%（3094/6403）降到 finerenone 33.9%（2174/6420），**HR 0.63（95% CI 0.60–0.66）**[label_guideline_safety_Pitt_2025]。這是 MRA class 的一致特徵：Jhund 2024 的 IPD meta（RALES/EMPHASIS/TOPCAT/FINEARTS，n=13,846）顯示 MRA 使低血鉀風險**減半（OR 0.51；95% CI 0.45–0.57；7% vs 14%）**[hf_renal_safety_Jhund_2024]。

**前提二：低血鉀本身確實與壞結局相關（且兩端皆害的 U 形）。** FIDELITY 中以病程最低血鉀分層，K<3.5（vs 恆≥4.0）對應 CV 複合 **HR 1.53（1.28–1.81）**、心律不整複合 **HR 1.67（1.31–2.13）**、全因死亡 **HR 1.56（1.27–1.91）**[label_guideline_safety_Pitt_2025]；FINEARTS-HF 的 **time-updated** 分析更顯示低血鉀端**風險甚至高於**高血鉀端——K<3.5 **HR 2.49（1.80–3.43）** > K>5.5 **HR 1.64（1.04–2.58）**[hf_renal_safety_Vardeny_2025]。

**但這兩個前提合起來，仍然只證明了「關聯」。** 關鍵在於：前提二裡「低血鉀 → 壞結局」的關聯是**觀察性、非隨機**的——沒有人被隨機分配「會不會低血鉀」，低血鉀的病人在利尿劑用量、心衰嚴重度、營養狀態上本就不同（見 [`statistical_insights_myths.md`](statistical_insights_myths.md) 迷思四所述 time-updated 分層的殘餘干擾）。低血鉀可能只是「病得更重」的**標記（risk marker）**，而非**致病的中介（mediator）**。要把「標記」升級成「中介」，必須證明**在 finerenone 的因果效應裡，有一部分是『經由血鉀這條路』傳遞的**——這正是下一節的工作。

---

## 🔬 因果中介的正式檢定（Agarwal 2026 四中介分析）——這是判決關鍵

Agarwal 2026 是目前唯一把**血鉀**放進正式 causal mediation framework 的分析，直接回答了 Pitt 留下的問號。設計：FIDELITY IPD（n=12,143），把 finerenone 在**第 4 個月**造成的四個 biomarker 變化同時當 mediator，檢定各自中介了多少 CV 複合益處（CV 死亡、非致死 MI、非致死中風、HHF；time-to-first）[albuminuria_mediation_Agarwal_2026]。四個 mediator 在第 4 月**都顯著改變**了：UACR 降 32.2%、SBP 降 3.6 mmHg、體重降 0.23 kg、而**血鉀上升 0.19 mEq/L（95% CI 0.17–0.20）**[albuminuria_mediation_Agarwal_2026]。

判決結果如下表——**「有沒有改變」與「有沒有中介」是兩回事**：

| Mediator（月 4 變化） | 顯著改變？ | 中介比例（含 treatment×mediator 交互） | 判定 |
|---|---|---|---|
| UACR ↓32.2% | 是 | **39%（95% CI 7 to 71）** | ✅ 顯著中介 |
| SBP ↓3.6 mmHg | 是 | **21%（95% CI 3 to 40）** | ✅ 顯著中介 |
| 體重 ↓0.23 kg | 是 | **4%（95% CI −1 to 9）** | ❌ 不顯著 |
| **血鉀 ↑0.19 mEq/L** | 是 | **−1.5%（95% CI −38 to 7）** | ❌ **不顯著（點估計為負）** |

[albuminuria_mediation_Agarwal_2026]

UACR 與 SBP **合併**中介了 **50%（95% CI 21 to 100）** 的 CV 益處[albuminuria_mediation_Agarwal_2026]；作者對血鉀的結論是**直白的反證**：「the protocol-permitted serum potassium increase **did not mediate** the cardiovascular benefit」[albuminuria_mediation_Agarwal_2026]、且「body weight and serum potassium are **not useful surrogates** for cardiovascular benefit」[albuminuria_mediation_Agarwal_2026]。

> **淺白比喻**：作者做的正是「切斷中間那一環，看益處會不會跟著消失」的思想實驗。UACR 這一環被切斷，益處掉了 39%——所以它**是**中介；血鉀這一環被切斷，益處**紋風不動**（點估計甚至 −1.5%）——所以血鉀**不是**傳遞益處的路徑，它只是 MR 阻斷這個共同上游**順帶**產生、與臨床益處**並存但不相連**的下游。這是本命題最強的一塊反證：不是「沒去驗」，而是**驗了、且驗出血鉀不中介**。

剩下那一半（約 50%）CV 益處**不被這四個系統性 biomarker 捕捉**，作者歸因於 MR 阻斷對心肌、巨噬細胞、血管壁的**直接抗纖維化與抗發炎效應**[albuminuria_mediation_Agarwal_2026]。換言之，finerenone 的益處主幹來自**組織層面的直接作用**（部分經 UACR/SBP 顯影 + 一半經未知的抗纖維化路徑），血鉀不在這條主幹上。

兩個補強細節讓這個判決更穩：(a) **穩健性**——UACR 的中介比例在納入交互時為 39%、不納入交互時為 **36%（95% CI 7 to 64）**[albuminuria_mediation_Agarwal_2026]，兩種模型一致，且對 mediator 測量誤差的敏感度分析亦穩定；血鉀的不顯著並非模型設定的偶然。(b) **時間軸也不支持血鉀路徑**——finerenone 的 CV 益處「emerges within months, before measurable kidney protection」[albuminuria_mediation_Agarwal_2026]（5 年 total effect 之 relative mean survival 1.12；95% CI 1.04 to 1.21）[albuminuria_mediation_Agarwal_2026]；益處在**腎保護可測之前**就已出現，指向的是**快速的直接組織效應**，而非需要時間累積的電解質再置中。這與「血鉀是主要中介」的圖像不相容。

---

## ⚖️ 收斂判決：血鉀高低「不決定、也不中介」finerenone 的 CV 益處

兩條獨立證據線在同一個結論上收斂：

1. **益處在高血鉀端仍維持（Vardeny 的「部分借隨機化」interaction 證據）。** FINEARTS-HF 用 time-updated Cox 比較「發生 K>5.5 之前 vs 之後」的 finerenone 相對益處：**HR 0.84（0.55–1.30）vs 0.83（0.74–0.92），interaction P = 0.72**[hf_renal_safety_Vardeny_2025]。摘要原文：「the clinical benefit associated with finerenone relative to placebo was **maintained even in those whose potassium level increased to greater than 5.5 mmol/L**」[hf_renal_safety_Vardeny_2025]。FIDELITY 平行印證：CV 益處 **HR 0.86（0.78–0.95），P-interaction 0.95**，跨基線血鉀次組**一致**[label_guideline_safety_Pitt_2025]。**若血鉀值真的決定臨床結局，益處早該在高血鉀端被抵消——但沒有。**

2. **血鉀在正式中介分析中不顯著（Agarwal 的因果證據）。** 如上，中介比例 −1.5%（95% CI −38 to 7），落在 0 的兩側[albuminuria_mediation_Agarwal_2026]。

**因此「低血鉀矯正 → 減少猝死」目前是一個「電生理上合理、但未被中介分析證實」的機制性外推，而非確立的因果中介。** 直覺的因果鏈沒有被證實，反而被兩個角度各自削弱：血鉀既不決定益處的大小（Vardeny），也不承載益處的傳遞（Agarwal）。

---

## 🧭 一個必須誠實做出的細緻區分：被反證的 ≠ 被檢定的全部

這是本檔最重要、也最容易被過度簡化的一點。Agarwal 2026 檢定的**不完全等於**本文標題那個狹義假說，兩者要分開講：

| 命題 | 被檢定的內容 | 現狀 |
|---|---|---|
| 「血鉀**淨變化**（實為小幅上升 +0.19 mEq/L）是否中介 **CV 複合終點**」 | Agarwal 2026 正式檢定 | **🟡 未支持中介**（中介 −1.5%，95% CI −38 to 7，未達顯著；「未達顯著」≠「證明零效應」，CI 寬）[albuminuria_mediation_Agarwal_2026] |
| 「finerenone 益處是否在高/低血鉀次組間**被修飾**」 | Pitt/Vardeny 的 interaction 檢定 | **🟡 已被反證**（P-interaction 0.95 / 0.72，益處一致）[label_guideline_safety_Pitt_2025][hf_renal_safety_Vardeny_2025] |
| 「**嚴重低血鉀的矯正**是否中介 **猝死（sudden death）**」 | — | **🔴 從未被任何正式 mediation 分析檢定** |

關鍵落差有二：(a) Agarwal 檢定的 mediator 是**全族群血鉀的淨變化**（一個小幅**上升** +0.19 mEq/L，反映 MR 阻斷的整體藥效），這**在概念上不同於**「finerenone 在原本會低血鉀的那一小群人身上把 K 拉回正常」這個**狹義的矯正效應**；(b) Agarwal 的因變數是 **CV 複合終點**，而非**猝死**這個單一硬終點——而低血鉀的電生理危害恰恰最可能落在猝死上。所以正確說法是：**「血鉀淨變化不中介 CV 複合」已被反證；「嚴重低血鉀矯正是否中介猝死」則尚未被檢定**，是一個開放的空缺，不能拿前者去宣稱後者、也不能拿「電生理合理」去填補它。

Vardeny 自己也留了一句誠實的機制性可能：「some of the benefits attributable to MRAs **may relate to** their reducing the risk for hypokalemia」[hf_renal_safety_Vardeny_2025]——注意這是「may relate to（可能有關）」的**假說措辭**，不是中介的證明，正好標定了目前證據的天花板。

---

## 💡 臨床意涵：別把「血鉀正常化」當成 finerenone 有效的替代指標

- **益處的主幹是 MR 阻斷的直接組織效應**（部分經 UACR/SBP 中介 + 約一半來自未被捕捉的抗纖維化/抗發炎路徑）[albuminuria_mediation_Agarwal_2026]；**減少低血鉀是真實但並存（parallel）的安全性益處**，不是療效的主要機轉。
- **不要用血鉀當療效替代指標。** 因為 finerenone 的藥效端點是**血鉀小幅上升**（+0.19 mEq/L）而非下降，把「血鉀漂亮/正常化」讀成「藥在起作用」會**方向性地誤導**；Agarwal 明言體重與血鉀**不是有用的 surrogate**[albuminuria_mediation_Agarwal_2026]。真正該追蹤的並行療效訊號是**月 4 的 UACR 與 SBP 反應**[albuminuria_mediation_Agarwal_2026]。
- **這反而讓 benefit-risk 更清爽。** 正因為血鉀不中介益處，高血鉀端出現的 K>5.5（Vardeny 中 finerenone HR 2.16）[hf_renal_safety_Vardeny_2025] 是一個**可用劑量調整/監測獨立管理的安全性議題**，管理它**不會犧牲療效**——這正是「permitted potassium increase 不減損 CV 保護」所支撐的處方安心感（NNT/NNH 權衡見 [`benefit_risk_discussion_nnt_nnh.md`](benefit_risk_discussion_nnt_nnh.md)）。
- **低血鉀端仍要顧，但理由是「低血鉀本身有害」而非「矯正它=療效」。** finerenone 內建的保鉀效應對併用排鉀利尿劑者是真實優點（見 [`hypokalemia_bidirectional_electrolyte.md`](hypokalemia_bidirectional_electrolyte.md)）——把它定位成安全性紅利，而不是療效機轉。

---

## 🔴 誠實邊界（Evidence limits）

- **無「hypokalaemia 矯正 → 猝死下降」的專屬正式 mediation 分析。** 現有最接近的 Agarwal 2026 檢定的是「血鉀淨變化 → CV 複合」，**非**「嚴重低血鉀矯正 → 猝死」；後者是 🔴 未檢定的空缺，本檔不對它下任何因果結論。
- **所有現有證據為 post hoc / 觀察性 / 次分析。** Agarwal 為 prespecified **post hoc** causal mediation[albuminuria_mediation_Agarwal_2026]；Pitt 為 exploratory/post hoc FIDELITY 次分析[label_guideline_safety_Pitt_2025]；Vardeny 的 time-updated 血鉀-結局關聯為**非隨機、條件式暴露**，僅「發生 K>5.5 前後」的 interaction 部分借力於隨機化[hf_renal_safety_Vardeny_2025]。
- **中介比例的 CI 很寬。** UACR 39%（7–71）、SBP 21%（3–40）、聯合 50%（21–100）[albuminuria_mediation_Agarwal_2026]——上界觸及 100% 表示精確度有限；「一半」是點估計而非窄區間。因果中介另依賴**無未測混淆的 mediator-outcome 關係**這一不可檢驗假設，屬 🟡 方法學保留。
- **外推限制。** 具體數字專屬 FIDELITY（CKD+T2D）與 FINEARTS-HF（HFmrEF/HFpEF）；Jhund 的 class 一致性（低血鉀減半、益處跨 EF 譜）[hf_renal_safety_Jhund_2024] 支持方向外推，但個別 mediation 比例不宜跨族群搬用。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|---|---|---|
| finerenone 減少低血鉀（K<3.5 HR 0.46；K<4.0 HR 0.63）＋ 低血鉀與壞結局相關（U 形） | 🟡 post hoc | `label_guideline_safety_Pitt_2025`、`hf_renal_safety_Vardeny_2025` 📄 |
| **血鉀淨變化不中介 CV 複合**（中介 −1.5%，95% CI −38 to 7）；UACR 39%+SBP 21%=聯合 50% | 🟡 因果中介 | `albuminuria_mediation_Agarwal_2026` 📄 |
| 益處在高血鉀端仍維持（before/after K>5.5：HR 0.84 vs 0.83，P-int 0.72；FIDELITY P-int 0.95） | 🟡 次分析（部分借隨機化） | `hf_renal_safety_Vardeny_2025`、`label_guideline_safety_Pitt_2025` 📄 |
| MRA class 一致：低血鉀減半（OR 0.51；7% vs 14%）、益處跨 EF 譜（複合 HR 0.77） | 🟡 IPD meta | `hf_renal_safety_Jhund_2024` 📄（📌 僅結構化 abstract） |
| 「嚴重低血鉀矯正 → 猝死」之專屬中介 | 🔴 **從未被檢定** | —（誠實揭露） |

---

## 本地全文語料（可 grep 稽核）

📄 全文：`albuminuria_mediation_Agarwal_2026`（四中介 causal mediation：n=12,143、UACR 39%、SBP 21%、體重 4%、**血鉀 −1.5%**、聯合 50%、"did not mediate"、"not useful surrogates"、月 4 各 mediator 變化 32.2%/3.6/0.23/+0.19）、`label_guideline_safety_Pitt_2025`（K<3.5 HR 0.46、K<4.0 HR 0.63、min-K CV 1.53/心律不整 1.67/死亡 1.56、CV/心律不整 −14%/−13%、P-int 0.95、心律不整複合含 sudden cardiac death、"not known if...mediated by the prevention of hypokalaemia"）、`hf_renal_safety_Vardeny_2025`（K<3.5 HR 0.46、time-updated 2.49 vs 1.64、before/after K>5.5 HR 0.84 vs 0.83 P-int 0.72、"maintained even in those whose potassium level increased"、"may relate to...reducing hypokalemia"）、`hf_renal_safety_Jhund_2024`（OR 0.51、7% vs 14%、複合 HR 0.77、n=13,846）。

> 注：`hf_renal_safety_Jhund_2024` 本地檔為 Europe PMC 結構化 **abstract**（全文非 OA、無 PMCID），故其數字標 📌；其餘三檔為 📄 全文。

---

## References（Vancouver 風格，含本地檔）

1. Agarwal R, Filippatos G, Pitt B, et al. Systolic blood pressure and albuminuria reduction mediate cardiovascular benefits of finerenone in type 2 diabetes and CKD (causal mediation analysis of FIDELITY). Nephrol Dial Transplant. 2026. 📄 [albuminuria_mediation_Agarwal_2026]
2. Pitt B, Agarwal R, Anker SD, et al. Hypokalaemia in patients with type 2 diabetes and chronic kidney disease: the effect of finerenone — a FIDELITY analysis. Eur Heart J Cardiovasc Pharmacother. 2025;11(1):11–19. 📄 [label_guideline_safety_Pitt_2025]
3. Vardeny O, Vaduganathan M, Claggett BL, et al. Finerenone, Serum Potassium, and Clinical Outcomes in Heart Failure With Mildly Reduced or Preserved Ejection Fraction (FINEARTS-HF). JAMA Cardiol. 2025;10(1). 📄 [hf_renal_safety_Vardeny_2025]
4. Jhund PS, Talebi A, Henderson AD, et al. Mineralocorticoid receptor antagonists in heart failure: an individual patient level meta-analysis (RALES/EMPHASIS/TOPCAT/FINEARTS). Lancet. 2024. 📌 abstract only [hf_renal_safety_Jhund_2024]

---
*此檔為主題五之因果推論專論，撰寫日期基準 2026-07-12。所有具體數字均可 grep 回上列本地全文 MD。核心判決：現有證據**不支持**血鉀（高或低）為 finerenone CV 益處的主要中介變項——(a) 益處在 K>5.5 仍維持（Vardeny，P-int 0.72）；(b) 血鉀淨變化在正式中介分析中不顯著（Agarwal，−1.5%）。**已被反證者**：血鉀淨變化不中介 CV 複合、益處不被血鉀次組修飾。**尚未被檢定者（🔴 誠實空缺）**：嚴重低血鉀『矯正』是否中介『猝死』從無專屬 mediation 分析，「低血鉀矯正→減少猝死」仍屬電生理合理但未證實之外推。臨床協定與雙向電解質描述見同資料夾各檔，本檔刻意互補不重複。*
