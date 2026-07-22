# 統計迷思與深度解讀 · 主題三（combination／mediation／短期替代終點的統計）

> 本檔為主題 03（第四支柱還是提早聯用）之**統計深度解讀**，把「同步聯用」試驗（CONFIDENCE 及其三篇次分析）裡最容易被床邊誤讀的統計，用「❌ 常見誤解 → ✅ 統計正解 → 💡 臨床亮點」三段式拆開。目標讀者為專科醫師；統計詮釋可以延伸、可以有創意，但**每個具體數字／HR／OR／R²／%／CI／mediation 比例都可 grep 回本地全文 MD**。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（不對其未載內容作具體斷言）。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織、改寫與**統計詮釋**；作者／年份／數字均出自本地 MD 檔。
>
> **證據分層**：🟢 方法學共識／已確立｜🟡 post hoc／次分析／surrogate／模型（exploratory）｜🔴 假說（hypothesis-generating，尚待專屬 RCT）。
>
> **經典錨點**：本檔以「相對風險 vs 絕對風險」這個最古老的統計迷思為**教學錨點**——同一個 HR，在不同基線風險的人身上換算出的絕對受益天差地別（見主題四 `methodology_subgroup_relative_vs_absolute.md`：statin RRR 29.2% 一致，但 ARR 從 1.5% 到 14.6%）。本主題把這個「相對數字很穩、但意義要換算」的直覺，延伸到 combination 試驗特有的四個統計陷阱：**中介比例的不對稱、P 值的沉默、替代終點的外推、以及『加成』到底是不是『超加成』**。

---

## 迷思 1｜三臂設計的「額外益處」怎麼歸因——eGFR-mediation 的不對稱是機轉指紋，不是雜訊

**錨點延伸**：相對 vs 絕對是問「同一個效果、換算到不同人身上差多少」；這裡的三臂 mediation 問的是更深的一層——「同一個 combination 的額外效果，拆開來是**哪條路**造成的」。

### ❌ 常見誤解
「combination 的 UACR 多降一截，不就是兩個藥各自壓球內壓、血流動力學疊加嗎？加 empa 跟加 finerenone 應該對稱，反正都是把腎絲球壓力再降一點。」

### ✅ 統計正解
CONFIDENCE 的因果中介分析（N=790 evaluable、690 進入 mediation）明確顯示**方向不對稱**：把 empagliflozin 加到 finerenone 之上，其 UACR 益處中**急性 eGFR 變化只中介 28%（P=0.07）**；反過來把 finerenone 加到 empagliflozin 之上，急性 eGFR 變化**只中介 5.2%（P=0.23）** [confidence_egfr_mediation_Agarwal_2026]。原文把這對照講得很白：combination 較 finerenone 單藥多降的 29% UACR「was partially mediated by the acute change in eGFR」，而較 empagliflozin 單藥多降的 32% 則「almost entirely independent of the acute eGFR change」[confidence_egfr_mediation_Agarwal_2026]。急性 eGFR 下降本身也不對稱：combination −26.6、finerenone −22.1、empagliflozin −24.8 mL/min/1.73 m²（P<0.001），且在**基線 eGFR 較高與使用利尿劑者**更明顯（兩者 P<0.001）[confidence_egfr_mediation_Agarwal_2026]。

**統計上必須誠實的邊界**：這是 exploratory 分析，原文自陳「Owing to the exploratory nature of the mediation analysis, wide CIs, and P values above 0.05, the results should be interpreted with a degree of caution」[confidence_egfr_mediation_Agarwal_2026]——兩個中介百分比的 P 值都 >0.05、CI 很寬。所以「28% vs 5.2%」的**方向**可信（兩藥血流動力學重疊程度不同），但**精確點值**不宜當硬數字宣讀。

### 💡 臨床亮點
把 mediation 想成「拆帳單」：加 empa 的帳單裡約三成是「血流動力學（壓球內壓）」這個項目，加 finerenone 的帳單裡這個項目幾乎是零——意味 finerenone 疊加的價值**幾乎全來自非血流動力學**的抗發炎／抗纖維化通路。這在床邊有兩個轉換：（1）finerenone 和 SGLT2i 是**機轉互補而非重複**，不是「兩個都在壓同一個壓力」；（2）看到 finerenone 起始後 eGFR 只輕微 dip、不像 SGLT2i 那樣明顯，**不代表它沒在保護腎臟**——它的保護本來就不寫在急性血流動力學這條路上。

---

## 迷思 2｜「未放大高血鉀」的 P 值——沉默不是清白，absence of evidence ≠ evidence of absence

**錨點延伸**：相對 vs 絕對教我們「一個數字要換算才有意義」；P 值迷思教我們「一個**不顯著**的數字，也要問它有沒有能力顯著」。

### ❌ 常見誤解
「CONFIDENCE 顯示同步加上 SGLT2i，高血鉀跟 finerenone 單藥比 P=0.91、P=0.85 都不顯著——太好了，**證明**同步聯用不會多出高血鉀，SGLT2i 把 finerenone 的鉀抵消掉了。」

### ✅ 統計正解
兩個 P 值講的是「**沒偵測到差異**」，不是「證明沒有差異」。CONFIDENCE 高血鉀次分析：combination vs finerenone 在**血鉀平均變化 P=0.91**、在**高血鉀 odds P=0.85**，皆無顯著差異 [confidence_trial_Agarwal_2026]。但把絕對率攤開看，combination 與 finerenone 幾乎一樣高、都遠高於 empagliflozin：整體高血鉀 113 人（14.5%）＝ combination 40/265（15.1%）、finerenone 48/255（18.8%）、empagliflozin 25/259（9.7%）[confidence_trial_Agarwal_2026]。更關鍵的證據在 OR——相對於 empagliflozin，combination 的 aOR 2.69（95% CI 1.46–4.96）與 finerenone 的 aOR 2.56（95% CI 1.42–4.59）**幾乎重疊** [confidence_trial_Agarwal_2026]：同步加上 SGLT2i 後，升鉀的 OR 沒有往下掉。

為什麼「不顯著」在這裡特別不能當「沒差」？原文自己點出三個 power 限制：finerenone 本身只讓血鉀升約 +0.18 mEq/L，「roughly one-third less than…spironolactone」，而「This smaller potassium excursion may have limited the opportunity to detect a mitigating effect of empagliflozin」；因此「the absence of a demonstrable reduction in hyperkalemia risk should be viewed as hypothesis-generating rather than definitive」[confidence_trial_Agarwal_2026]。加上這是 180 天短試驗、事件數少（總共 113 件），而且**主要終點是 UACR、不是高血鉀安全性**——這個分析從設計上就不是為了偵測血鉀差異而 power 的。Wen 統合也印證：combination vs finerenone 的高血鉀 OR 1.09（95% CI 0.52–2.28、I²=95.1%），CI 寬到 1 兩側都涵蓋，根本不是「等效」的證據 [hyperkalemia_combo_Wen_2026]。

### 💡 臨床亮點
把 P=0.91／0.85 正確翻譯成「**同步起始 SGLT2i 並沒有幫你把 finerenone 的高血鉀抵消掉**」，而不是「聯用很安全不用管鉀」。床邊決策：同步聯用時，血鉀監測節奏**照 finerenone 單藥的規格走**（起始／增量後 4 週複測），不能因為「加了 SGLT2i」就鬆手。真正可能降鉀的情境是「**SGLT2i 先行、讓遠端小管適應後再加 finerenone**」——FIVE-STAR 次分析中，非 SGLT2i 背景加 finerenone 升鉀 +0.37 mEq/L，已在 SGLT2i 背景者只升 +0.13 mEq/L（P-interaction 0.02）[hyperkalemia_combo_Sinclair_2026]，但這是**非隨機、hypothesis-generating** 🔴，與 CONFIDENCE「同步不抵消」並不矛盾（時序不同）。

---

## 迷思 3｜180 天 UACR 是替代終點——「更大 UACR 降幅」到「更少腎衰」中間隔著一次外推

**錨點延伸**：相對 vs 絕對是「同一終點、換算單位」；替代終點迷思更進一步——「**換了一個終點**，還能不能推回真正在乎的硬結局」。

### ❌ 常見誤解
「combination 把 UACR 從基線降 52%（vs finerenone 32%、empagliflozin 29%），比單藥多降 29–32%——那長期腎衰、洗腎當然也會等比例少掉。UACR 降這麼多，硬結局跟著贏是理所當然。」

### ✅ 統計正解
CONFIDENCE 主要終點是「**Day 180 的 log-UACR 相對變化**」，是一個 180 天的**替代終點**，不是 kidney failure/doubling creatinine/renal death [combination_editorial_Cheng_2025][confidence_trial_Agarwal_2026]。「UACR 多降 → 腎衰少」是一次**surrogate-based 外推**，其正當性建立在外部證據：2019 年 41 試驗、29,979 人的病人層級統合顯示，前 6 個月**≥30% albuminuria 下降**對應長期腎複合終點風險**降 27%（HR 0.73；95% CI 0.67–0.81）**（median 3.4 年、3935 事件）[combination_editorial_Georgianos_2025]。CONFIDENCE 過半受試者在各 KDIGO 風險層都跨過這個 >30% 門檻（very high 層 70.6%）[confidence_trial_Vaduganathan_2025]。

但外推有硬邊界，且統計上有兩個「為什麼不能直接做硬終點試驗」的理由：（1）一個為偵測硬腎終點差異而 power 的 Phase 3，估計需隨機化**約 41,000 人**，可預見的未來不會有 [combination_editorial_Georgianos_2025]；（2）直接檢驗硬終點的統合尚未跨過門檻——Wen 的 trial sequential analysis 顯示，combination vs SGLT2i 單藥的 all-cause mortality（OR 0.73；0.47–1.13）、MACE（OR 0.77；0.55–1.08）、MAKE（OR 0.87；0.58–1.31）**皆不顯著**，累積 Z 曲線「did not cross trial sequential monitoring boundaries for benefit nor enter futility zone」[hyperkalemia_combo_Wen_2026]。所以「combination 在硬結局上優於 SGLT2i 單藥」目前是 surrogate 推論、**不是已證實的事實**。

### 💡 臨床亮點
UACR 是很好的**治療優化訊號**（降得多、降得快、可回溯風險），值得拿來 titrate 與打破 therapeutic inertia；但要對病人／同儕誠實：這是「**代理終點上的勝利**」，硬終點的加成**尚未有專屬 outcome trial**。床邊語言：把 combination 定位成「更快讓 UACR 進入低風險帶、爭取時間」，而非「已證明多救多少顆腎」。這一段的 surrogate 邏輯與主題二一脈相承（albuminuria 作為 mediator 的因果強度見主題二）。

---

## 迷思 4｜「additive」還是「over-additive」——臨床的『超加成』沒有做過正式交互檢定

**錨點延伸**：相對 vs 絕對是「別把相對當絕對」；這裡是「**別把『比單藥好』當成統計證明的『超加成』**」——兩者是不同的統計主張。

### ❌ 常見誤解
「preclinical 老鼠實驗看到 empa+finerenone 對蛋白尿是『over-additive（超加成）』，CONFIDENCE 又看到 combination 比兩個單藥都好，所以人身上也**統計證實了協同 synergy**。」

### ✅ 統計正解
要分清三個層次。（a）**preclinical**：高血壓終末器官損傷大鼠中，低劑量 combination 產生「premature, sustained, and over-additive reduction in albuminuria」，7 週存活率也顯著較高 [combination_editorial_Georgianos_2025]——這是動物、劑量與物種都需外推。（b）**臨床「比單藥好」**：CONFIDENCE 中 combination vs finerenone LS mean ratio 0.71（0.61–0.82）、vs empagliflozin 0.68（0.59–0.79），皆 P<0.001 [combination_editorial_Cheng_2025][confidence_trial_Vaduganathan_2025]——這證明的是「**優於各單藥（additive/beat-each-monotherapy）**」。（c）**統計上的『超加成』**：需要一個 2×2 factorial 設計去檢定「合併效果 > 兩單藥效果的加總／相乘」，CONFIDENCE 是三臂平行、**並非為 super-additivity 的正式交互檢定而設計**，也沒有報這個 interaction P 值。文獻裡出現的 P_interaction 是**另一回事**——Vaduganathan 測的是「combination 相對益處在 KDIGO 風險層間是否一致」，得 P_interaction >.05（very high 層 LSMR 0.72／0.75）[confidence_trial_Vaduganathan_2025]，這檢定的是「跨風險層一致性」，不是「超加成」。而且該分析明載「No adjustment for multiple comparisons was made」[confidence_trial_Vaduganathan_2025]。

### 💡 臨床亮點
講給同儕聽時，用「**明確優於任一單藥、且跨風險層一致**」這個站得住的說法，而不是浮誇的「協同 synergy」。臨床決策不需要「超加成」成立——「combination 比兩個單藥各自都好、且不論病人腎風險高低都好」已足以支持「不必等到極高風險才聯用」。但把「over-additive」當成已被人體正式檢定的統計結論來衛教，會超出資料能承擔的範圍；那個詞的最強證據仍在**動物模型** 🔴。

---

## 迷思 5｜三臂試驗的「乾淨隨機」——別把 subgroup 的 confounding by indication 帶進 CONFIDENCE 的結論

**錨點延伸**：相對 vs 絕對提醒「數字要放回它的分母」；這裡提醒「**結論要放回它的設計**」——同一個問題，隨機化的答案與觀察性的答案份量不同。

### ❌ 常見誤解
「FIDELITY 次分析看到『基線有用 SGLT2i 的人高血鉀較少（10.3% vs 未用 14.3%）』，所以 SGLT2i 一定會降 finerenone 的鉀——CONFIDENCE 沒看到，八成是 CONFIDENCE 有問題。」

### ✅ 統計正解
兩者不矛盾，差別在**設計**與**時序**。FIDELITY 的 SGLT2i 亞組是 **prespecified pooled analysis**，但「是否使用 SGLT2i」本身**非隨機分派**：基線用 SGLT2i 者本來就腎功能較好（mean eGFR 66.3 vs 57.0 mL/min/1.73 m²）、UACR 較低（median 448 vs 521 mg/g）、GLP-1RA 使用率高約三倍（19.0% vs 6.4%）[sglt2i_subgroup_FIDELITY_Rossing_2022]——這是典型的 **confounding by indication**，所以只能看 P_interaction、不能拿組間點估計當因果。CONFIDENCE 的三臂 1:1:1 隨機化是**唯一沒有這個偏誤**的設計，而它的答案是「同步起始不抵消高血鉀」（P=0.91／0.85）[confidence_trial_Agarwal_2026][hyperkalemia_combo_Sinclair_2026]。兩者的**時序不同**（FIDELITY 是慢性 SGLT2i 背景、CONFIDENCE 是同步起始），正好被 FIVE-STAR 的 P-interaction 0.02（+0.37 vs +0.13 mEq/L）串起來 [hyperkalemia_combo_Sinclair_2026]——降鉀效應可能需要 SGLT2i 先「適應」一段時間。

### 💡 臨床亮點
證據階層的床邊用法：當隨機化證據（CONFIDENCE）與觀察性訊號（FIDELITY 亞組）方向不一致時，**以隨機化為準**，把觀察性訊號降級為「可能的時序假說」。實務結論：想靠 SGLT2i 降 finerenone 的鉀，**「先 SGLT2i、後 finerenone」在機轉上較有指望**，但這仍需 Sinclair 呼籲的三臂 sequencing RCT（finerenone-first／同步／SGLT2i-first、以血鉀變化為主終點）來證實 🔴 [hyperkalemia_combo_Sinclair_2026]。

---

## 統計素養檢查表（簡報／查房一頁）

| 看到這個 | 先問這句 | 本主題的具體例 |
|---|---|---|
| 一個亮眼的相對降幅（UACR −52%） | 換算成硬結局的絕對受益要幾步外推？ | 180 天 UACR 是 surrogate，硬終點需 ~41,000 人 RCT [combination_editorial_Georgianos_2025] |
| 一個「不顯著」的安全性 P 值（P=0.91／0.85） | 這個分析**有沒有 power** 偵測差異？主終點是不是它？ | 主終點是 UACR、事件僅 113、finerenone 升鉀本就小 → absence of evidence [confidence_trial_Agarwal_2026] |
| 「combination 比單藥好」 | 是「優於單藥」還是「正式檢定的超加成」？ | 無 2×2 factorial super-additivity 檢定；over-additive 最強證據在動物 [combination_editorial_Georgianos_2025] |
| mediation 百分比（28% vs 5.2%） | exploratory 嗎？CI 多寬？P 過 0.05 嗎？ | 兩者 P 皆 >0.05、CI 寬 → 讀方向不讀點值 [confidence_egfr_mediation_Agarwal_2026] |
| 一個 P_interaction | 它檢定的是「一致性」還是「加成」還是「效果修飾」？校正多重了嗎？ | Vaduganathan P_interaction >.05 是跨風險層一致性、未校正多重 [confidence_trial_Vaduganathan_2025] |
| 觀察性亞組的組間差（10.3% vs 14.3%） | 有 confounding by indication 嗎？該看點估計還是 P_interaction？ | FIDELITY 有用 SGLT2i 者基線 eGFR 較好 → 只能看 P_interaction [sglt2i_subgroup_FIDELITY_Rossing_2022] |

---

## 證據分層小結

| 統計論點 | 等級 | 主要本地全文來源 |
|---|---|---|
| eGFR-mediation 不對稱（加 empa 28% vs 加 fine 5.2%）→ 兩藥血流動力學重疊程度不同 | 🟡 exploratory（P>0.05、CI 寬） | `confidence_egfr_mediation_Agarwal_2026` 📄 |
| 同步聯用未放大高血鉀（P=0.91／0.85）屬 absence of evidence，非 evidence of absence | 🟡→🔴（未 power、主終點非安全性） | `confidence_trial_Agarwal_2026`、`hyperkalemia_combo_Wen_2026` 📄 |
| 180 天 UACR → 硬結局為 surrogate-based 外推（≥30% ↓ ↔ HR 0.73） | 🟡 surrogate | `combination_editorial_Georgianos_2025`、`combination_editorial_Cheng_2025` 📄 |
| 「優於單藥」已證、「超加成」未做正式交互檢定 | 🟡（臨床優於單藥）／🔴（超加成僅 preclinical） | `combination_editorial_Georgianos_2025`、`confidence_trial_Vaduganathan_2025` 📄 |
| 硬終點 additivity 未跨 TSA 邊界（mortality/MACE/MAKE 皆不顯著） | 🔴 尚待 RCT | `hyperkalemia_combo_Wen_2026` 📄 |
| 時序假說（SGLT2i 先行降鉀，+0.37 vs +0.13，P-int 0.02） | 🔴 hypothesis-generating（非隨機） | `hyperkalemia_combo_Sinclair_2026` 📄 |

## 本地全文語料（可 grep 稽核）

📄 全文：`confidence_egfr_mediation_Agarwal_2026`（JASN，eGFR 中介 28%／5.2%、急性 dip 26.6/22.1/24.8）、`confidence_trial_Agarwal_2026`（JACC，高血鉀 P=0.91/0.85、15.1%/18.8%/9.7%、aOR 2.69/2.56、「absence…hypothesis-generating」）、`confidence_trial_Vaduganathan_2025`（KDIGO 風險層一致性、LSMR 0.72/0.75、未校正多重）、`combination_editorial_Georgianos_2025`（~41,000 人、2019 統合 HR 0.73、preclinical over-additive）、`combination_editorial_Cheng_2025`（UACR 52%/32%/29%、LSMR 0.71/0.68）、`hyperkalemia_combo_Wen_2026`（OR 1.09/3.00、mortality/MACE/MAKE 不顯著、TSA）、`hyperkalemia_combo_Sinclair_2026`（FIVE-STAR +0.37/+0.13、P-int 0.02、sequencing RCT 呼籲）、`sglt2i_subgroup_FIDELITY_Rossing_2022`（confounding by indication 基線量化）。

---

## References（本地可稽核）

1. Agarwal R, Correa-Rotter R, Navaneethan SD, et al. Acute eGFR changes and their mediation of albuminuria reduction with empagliflozin and finerenone (CONFIDENCE). *J Am Soc Nephrol.* 2026. 📄 [confidence_egfr_mediation_Agarwal_2026]
2. Agarwal R, Green JB, Heerspink HJL, et al. Risk of hyperkalemia with empagliflozin, finerenone, or both: secondary analysis of the CONFIDENCE randomized trial. *J Am Coll Cardiol.* 2026;87(7):772–784. 📄 [confidence_trial_Agarwal_2026]
3. Vaduganathan M, Green JB, Heerspink HJL, et al. Simultaneous initiation of finerenone and empagliflozin across the spectrum of kidney risk in the CONFIDENCE trial. *Nephrol Dial Transplant.* 2026;41(1):161–170. 📄 [confidence_trial_Vaduganathan_2025]
4. Georgianos PI, Koufakis T, Arampatzis S, Liakopoulos V. CONFIDENCE in the safety and efficacy of dual therapy with an SGLT-2 inhibitor and finerenone. *Diabetes Obes Metab.* 2025;27(11):6097–6100. 📄 [combination_editorial_Georgianos_2025]
5. Cheng AYY, Mottl A, Magwire M. Pillar risk-based treatment for CKD in people with type 2 diabetes: a narrative review. *Diabetes Ther.* 2025;16(11):2083–2099. 📄 [combination_editorial_Cheng_2025]
6. Wen CF, Chuang MH, Wu VC, Chen JY. Efficacy of combined SGLT2 inhibitors and finerenone in CKD: a systematic review and meta-analysis. *Front Pharmacol.* 2026;17:1803971. 📄 [hyperkalemia_combo_Wen_2026]
7. Sinclair MR, Edmonston D. It's about time: potassium risk with combination guideline-directed medical therapy. *Kidney Int Rep.* 2026;11:106609. 📄 [hyperkalemia_combo_Sinclair_2026]
8. Rossing P, Anker SD, Filippatos G, et al. Finerenone by SGLT2 inhibitor treatment: the FIDELITY analysis (baseline characteristics). *Diabetes Care.* 2022;45(12):2991–2998. 📄 [sglt2i_subgroup_FIDELITY_Rossing_2022]

---
*此檔為主題三之統計深度解讀，撰寫日期基準 2026-07-11。所有具體數字（28%/5.2%、P=0.91/0.85、15.1%/18.8%/9.7%、aOR 2.69/2.56、LSMR 0.71/0.68、HR 0.73、OR 1.09/3.00、+0.37/+0.13、P-int 0.02）均可 grep 回上列本地全文 MD。四項明示邊界：(a) mediation 為 exploratory、P>0.05、CI 寬，讀方向不讀點值；(b) 高血鉀「不顯著」屬未 power 的 absence of evidence；(c) 180 天 UACR 為 surrogate，硬終點加成未有專屬 RCT；(d)「over-additive」之人體正式交互檢定不存在，其最強證據在 preclinical。*
