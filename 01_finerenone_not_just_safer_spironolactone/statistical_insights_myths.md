# 統計迷思與深度解讀 · 主題一(機轉→生物標記→臨床的統計橋樑)

> 本檔為主題 01(finerenone 不只是比較安全的 spironolactone)之**統計深度解讀**,把主文「三層對讀」(分子機轉→生物標記→臨床表型)背後最容易被誤讀的統計環節獨立拆出,聚焦一個核心問題:**當我們從一個分子數字(結合親和力、選擇性倍數)或一個生物標記(UACR、NT-proBNP、風險分數)去推論「臨床上對病人有多少好處」時,統計上會踩到哪些坑?**
>
> **引用標記慣例**:📄 = 本地全文可 grep 稽核;📌 = 僅取得 abstract(不對其未載內容作具體數字斷言)。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織、改寫與**統計詮釋**;所有作者、年份、數字均出自本地 MD 檔,詮釋可延伸,數字不可杜撰。
>
> **證據分層**:🟢 已確立的方法學共識 / RCT 主終點｜🟡 post hoc / 次分析 / surrogate / mediation｜🔴 假說、機轉外推、in-vitro。
>
> **經典錨點:相對風險 vs 絕對風險。** 全檔以這個最古老的統計迷思當作校準尺——「打幾折(相對效果 / HR)」在不同病人身上通常很穩定,但「省多少錢(絕對效果 / ARR、NNT)」會隨基線風險放大好幾倍。本主題把這把尺延伸到「分子→生物標記→臨床」這條轉譯鏈上,拆出四個專屬迷思。

---

## 錨點範例:同一個 HR,NNT 可以差 12 倍 🟢

**先用白話講**:finerenone 在 FINEARTS-HF 的相對效果幾乎「一視同仁」——不論病人基線風險高低,HR 都在 0.8–0.9 之間;但「值不值得開」不是看 HR,而是看**絕對受益**。

在 Chimura 的 FINEARTS-HF 次分析(6001 名 HFmrEF/HFpEF)中,用 EMPEROR-Preserved 風險模型把病人分成五等分,finerenone 的相對效果跨風險層一致(Q1→Q5 的 HR 分別 0.93、1.04、0.82、0.81、0.88,**P for interaction = .68**)[biomarker_Chimura_2026.md] 📄。但把「同一個整體相對風險下降」套回各層,最低風險 Q1 的絕對下降僅 **3.7 per 1000 person-years(NNT 272)**,最高風險 Q5 卻是 **43.0 per 1000 person-years(NNT 23)**——**同樣的 HR,NNT 差了近 12 倍** [biomarker_Chimura_2026.md] 📄。

> **💡 臨床亮點**:「HR 不變」不是「人人一樣受益」的證據,恰恰相反,它**保證**高風險病人的絕對受益更大。看到「跨亞群一致」的漂亮森林圖,正確反應是去算病人的基線絕對事件率,而不是把 HR 當成每個人都能拿到的折扣。這把尺會在下面四個迷思裡反覆出現。

---

## 迷思一:「500-fold 選擇性」是效益倍數? 🔴→🟢

**❌ 常見誤解**:finerenone 對 MR 的選擇性「至少 500 倍」,聽起來像是「比舊藥強 500 倍」「臨床效益是舊藥的好幾百倍」,於是把 in-vitro 的親和力比值直接當成床邊療效的放大倍數。

**✅ 統計正解**:選擇性倍數(fold-selectivity)是**藥理效價比**,量的是「這個分子多偏好 MR、多不去碰其他受體」,而**不是**「對硬終點有多少效益」。兩者根本是不同的量綱。Kolkhof 2017 的原文是:finerenone「is at least as potent as spironolactone and even more selective (at least 500-fold toward MR) than eplerenone」——注意它把**效價(potency)**與**選擇性(selectivity)**分開講:效價「至少與 spironolactone 相當」,選擇性才是「至少 500 倍」,且此選擇性是對照 65 個受體與離子通道(含 L-type Ca²⁺ channel)測出來的分子行為 [molecular_Kolkhof_2017.md] 📄。實際效價數字更能戳破倍數幻覺:finerenone 的 IC50 為 **58 ± 9 nM**、spironolactone **74.0 ± 15 nM**(Kd = **1.52 ± 0.01 nM**)——效價只差約 1.3 倍,而非幾百倍 [molecular_Amazit_2015.md] 📄。同理,esaxerenone 的「at least a 1000-fold higher selectivity for MR」也只是選擇性,不代表它臨床上比 finerenone 強 [molecular_Kolkhof_2017.md] 📄。

**💡 臨床亮點**:「高選擇性」正確的臨床翻譯是**副作用譜更乾淨**(不碰雄激素/黃體素受體 → 少男性女乳症),以及**分子行為可預測**(對 S810L 突變 MR 維持嚴格拮抗);而「有多少心腎保護」這一問,只能由 RCT 的 HR/NNT 回答,不能由 nM 或 fold 外推。把 500-fold 當作「療效證書」是把分子藥理學的尺拿去量臨床結局——量綱錯了。

---

## 迷思二:「BP-independent」是「沒降血壓」嗎? 🟡

**❌ 常見誤解**:把「效益獨立於血壓」理解成「finerenone 根本沒降血壓,所以效益跟血壓無關」。事實上它**有**降血壓——FIDELITY 第 4 個月 SBP −3.2 vs 安慰劑 +0.5 mmHg [biomarker_Agarwal_2022.md] 📄——只是幅度不大。

**✅ 統計正解**:「獨立」不是「沒有」,而是一個**中介分析(mediation)**的結論:把 SBP 這條路徑「扣掉 / 中介掉」之後,效益仍有一大半留著。Agarwal 2026 用 FIDELITY 個體資料(n = 12,143)做 causal mediation:第 4 個月 finerenone 降 UACR **32.2%**、降 SBP **3.6 mmHg**,但四個候選中介裡只有兩個真正中介了心血管效益——**UACR 中介 39%(95% CI 7 to 71)、SBP 中介 21%(3 to 40)**,體重與血鉀不中介;兩者合計中介 **50%(95% CI 21 to 100)** [biomarker_Agarwal_2026.md] 📄。換言之「BP-independent」的統計意涵是:**SBP 這條路只解釋了約 1/5 的效益,還有約一半的效益連 UACR+SBP 都無法解釋**,指向 MR 相關的抗發炎/抗纖維化等非血流動力學路徑。

**💡 臨床亮點**:這也劃出「獨立」的**邊界**——21% 不是 0%,降那 3.6 mmHg 確實貢獻了一部分,但你**不能靠加一顆降壓藥去複製 finerenone 的效益**,因為另外約 80% 走的是別條路。床邊決策:不要因為病人血壓已達標就認定 finerenone「沒必要」;它的主要價值不在那 3.6 mmHg。(先前單獨分析:UACR 單獨中介 37%、SBP 以 time-varying 法估 12.6%,合併後才看清重疊與互補 [biomarker_Agarwal_2026.md] 📄。)

---

## 迷思三:生物標記「分得出高低風險」= 對誰更有效? 🟡

**❌ 常見誤解**:看到 NT-proBNP 或風險模型「鑑別度很好、能把高低風險分得很開」,就推論「所以 finerenone 對高風險的人特別有效、對低風險的人沒效」。把**預後(prognosis)**當成了**療效預測(treatment effect modification)**。

**✅ 統計正解**:鑑別度(discrimination,如 Harrell C statistic)回答的是「模型能不能排出誰會出事」,與「finerenone 對誰的**相對**效果更大」是兩個獨立問題。Chimura 的 EMPEROR-Preserved 模型在 FINEARTS-HF 的鑑別度確實好——Q5 vs Q1 的事件 HR 高達 **10.49(95% CI 8.14–13.52)**(CV death 更達 **13.47**),且優於單用 NT-proBNP [biomarker_Chimura_2026.md] 📄。但**治療**效果跨五分位卻**平的**(P for interaction = .68,見上文錨點)[biomarker_Chimura_2026.md] 📄。所以「風險模型很會分人」推不出「藥對高風險更有效(相對尺度上)」;它推出的是**絕對受益梯度**(NNT 272 → 23)。另一個常被混淆的是「風險標記 vs 中介」:Lu 2026 顯示猝死前 6 個月 NT-proBNP 由約 **1800 升到 2000 pg/mL**,存活者則由約 **800 降到 650 pg/mL** [biomarker_Lu_2026.md] 📄——這是縱向**風險標記軌跡**(病情變差的伴隨現象),作者明言此為 population-level、hypothesis-generating [biomarker_Lu_2026.md] 📄,**不等於**「壓低 NT-proBNP 就等量換到存活」(那要中介分析才能宣稱,如迷思二)。

**💡 臨床亮點**:用生物標記/風險分數做的是兩件正確的事——(1)**選人與試驗富集**(挑絕對受益大的人),(2)**追蹤反應趨勢**(NT-proBNP 往上爬是預警);但**不要**用它來說「這個人風險低所以不必給藥」(相對效果一樣,只是絕對數字小),也**不要**把「NT-proBNP 降了」直接當「命救回來了」。

---

## 迷思四:「至少與 spironolactone 相當」是等效硬終點嗎? 🔴

**❌ 常見誤解**:把 ARTS 的「BAY 94-8862 降 BNP/NT-proBNP/UACR 至少與 spironolactone 相當」讀成「已經證明兩藥**療效等效**」,甚至「所以硬終點也會一樣」。這是把 non-inferiority 的語言、又是在 surrogate 上、又是 power 不足的 phase 2 結果,升級成了等效宣稱。

**✅ 統計正解**:ARTS 是 **phase II** 試驗,**主終點是血清鉀變化**,所有生物標記(BNP/NT-proBNP/UACR)都是「only exploratory」的次終點;而且原文寫得很白:part B「showed **no significant overall treatment effect on BNP, NT-proBNP, or urinary albumin:creatinine ratio (UACR) (P > 0.05)**, so P-values for individual treatment group comparisons were not calculated, and the treatment groups were analysed only descriptively」[arts_program_Pitt_2013.md] 📄。也就是說「至少相當」是**描述性觀察**,連正式檢定都沒做——它的樣本量是為了偵測 K⁺ 差 0.26 mmol/L 而算的(80% power),不是為了比生物標記 [arts_program_Pitt_2013.md] 📄。ARTS-HF 同理:**phase 2b**,主終點是「NT-proBNP 下降 >30% 的比例」,eplerenone 37.2% vs finerenone 各劑量 30.9–38.8%(**P = 0.42–0.88**),那個亮眼的臨床複合 HR 0.56(0.35–0.90)是**探索性、nominal P**,原文自陳「despite the fact that this phase 2 study was **not designed to detect statistical significant differences**」[arts_hf_Filippatos_2016.md] 📄。更關鍵的誠實話:主終點只是 surrogate,作者提醒「changes in natriuretic peptides by several drugs were **not related to improved outcome** in clinical trials」[arts_hf_Filippatos_2016.md] 📄。

**💡 臨床亮點**:「至少相當」在統計上是**沒有證明差異**(absence of evidence),不是**證明沒有差異**(evidence of absence)——尤其在 power 只夠比血鉀的試驗裡。床邊翻譯:ARTS/ARTS-HF 的正當結論是「finerenone 在**更小的高血鉀/腎功能惡化代價**下,拿到**至少不遜色**的生物標記反應,值得進 phase III」,而**不是**「兩藥療效等效、可互換」。finerenone 的硬終點地位來自 FIDELIO/FIGARO/FIDELITY 與 FINEARTS-HF 的**安慰劑對照**,而非任何對 spironolactone/eplerenone 的頭對頭等效證明(本主題全無此類長期硬終點對頭資料)。

---

## 統計素養檢查表(查房 / 簡報一頁用)

| 看到這個 | 先問這句 | 別掉進的坑 |
|---|---|---|
| 「選擇性 500 倍 / 親和力更高」 | 這是效價/選擇性(nM、fold),還是硬終點效益(HR/NNT)? | 把分子倍數當療效倍數(迷思一) |
| 「效益 BP-independent」 | 中介分析扣掉 SBP 後還剩多少?(SBP 僅約 21%) | 把「獨立」讀成「沒降壓」或「加降壓藥可複製」(迷思二) |
| 「風險模型鑑別度很好」 | 這是預後(誰會出事),還是療效預測(對誰更有效)? | 用預後模型排除低風險病人的**相對**效益(迷思三) |
| 「NT-proBNP 降了 / 軌跡上升」 | 這是風險標記,還是已證實的中介? | 把 surrogate 變化當成救命的等量兌換(迷思三、四) |
| 「至少與 X 相當」 | 是 powered 的 non-inferiority,還是描述性、P>0.05、surrogate? | 把「沒測到差異」升級成「等效硬終點」(迷思四) |
| 「跨亞群 HR 一致」 | 那絕對 ARR/NNT 呢?(NNT 可差 12 倍) | 把 HR 當成人人可得的折扣(錨點) |

---

## 證據分層小結

| 統計論點 | 等級 | 主要本地全文來源 |
|---|---|---|
| 同一 HR、NNT 差 12 倍(272 vs 23);相對一致 → 絕對放大 | 🟢/🟡 | `biomarker_Chimura_2026.md` 📄 |
| 選擇性/效價是分子量綱:IC50 58 vs 74 nM、選擇性「至少 500-fold」 | 🔴→🟢 | `molecular_Kolkhof_2017.md`、`molecular_Amazit_2015.md` 📄 |
| BP-independent = SBP 僅中介 21%、UACR 39%、合計 50% | 🟡 mediation | `biomarker_Agarwal_2026.md` 📄 |
| 鑑別度(Q5/Q1 HR 10.49)≠ 療效修飾(P-interaction .68) | 🟡 次分析 | `biomarker_Chimura_2026.md` 📄 |
| NT-proBNP 軌跡為風險標記(1800→2000 vs 800→650),非中介 | 🟡 post hoc | `biomarker_Lu_2026.md` 📄 |
| 「至少相當」為描述性 surrogate、P>0.05、非 powered 等效 | 🔴 phase 2 | `arts_program_Pitt_2013.md`、`arts_hf_Filippatos_2016.md` 📄 |
| finerenone vs 類固醇型 MRA 的長期硬終點對頭資料 | 🔴 尚無 | —(誠實揭露) |

## 本地全文語料(可 grep 稽核)

📄 全文:`molecular_Kolkhof_2017.md`(500-fold 選擇性、esaxerenone IC50 對照)、`molecular_Amazit_2015.md`(IC50 58/74 nM、Kd 1.52 nM、S810L 嚴格拮抗)、`biomarker_Agarwal_2026.md`(FIDELITY causal mediation:UACR 39% / SBP 21% / 合計 50%;round-2 上傳全文 PDF)、`biomarker_Chimura_2026.md`(EMPEROR-Preserved 風險模型、Q5/Q1 HR、NNT 272 vs 23、P-interaction .68)、`biomarker_Lu_2026.md`(死亡前 NT-proBNP 軌跡)、`arts_program_Pitt_2013.md`(ARTS phase II、K⁺ 主終點、生物標記 P>0.05 只描述性)、`arts_hf_Filippatos_2016.md`(ARTS-HF phase 2b、NT-proBNP >30% 主終點、HR 0.56 nominal)、`arts_program_Bakris_2015.md`(ARTS-DN、UACR 21–38% 劑量反應)。
佐證(見主文):`biomarker_Agarwal_2022.md`(FIDELITY SBP −3.2 vs +0.5)、`biomarker_Filippatos_2023.md`(效益大體與代謝因子無關)。

---

## References(Vancouver 風格,含本地檔)

1. Kolkhof P, Bärfacker L. 30 years of the mineralocorticoid receptor: MRAs — 60 years of research and development. J Endocrinol. 2017;234(1):T125-T140. 📄 [molecular_Kolkhof_2017.md]
2. Amazit L, Le Billan F, Kolkhof P, et al. Finerenone impedes aldosterone-dependent nuclear import of the mineralocorticoid receptor and prevents genomic recruitment of SRC-1. J Biol Chem. 2015;290(36):21876-21889. 📄 [molecular_Amazit_2015.md]
3. Agarwal R, et al. Systolic blood pressure and albuminuria reduction mediate cardiovascular benefits of finerenone in T2 diabetes and CKD (causal mediation, FIDELITY). Nephrol Dial Transplant. 2026. 📄 [biomarker_Agarwal_2026.md]
4. Chimura M, McDowell K, Jhund PS, et al. EMPEROR-Preserved risk model and outcomes in the FINEARTS-HF trial: a prespecified secondary analysis. JAMA Cardiol. 2026. 📄 [biomarker_Chimura_2026.md]
5. Lu H, Kosztin A, Claggett BL, et al. Biomarker, functional status, and quality-of-life trajectories before modes of death in heart failure: post hoc analysis of FINEARTS-HF. JAMA Cardiol. 2026. 📄 [biomarker_Lu_2026.md]
6. Pitt B, Kober L, Ponikowski P, et al. Safety and tolerability of the novel non-steroidal MRA BAY 94-8862 in patients with chronic heart failure and mild or moderate CKD (ARTS). Eur Heart J. 2013;34(31):2453-2463. 📄 [arts_program_Pitt_2013.md]
7. Filippatos G, Anker SD, Böhm M, et al. A randomized controlled study of finerenone vs. eplerenone in patients with worsening chronic heart failure and diabetes and/or CKD (ARTS-HF). Eur Heart J. 2016;37(27):2105-2114. 📄 [arts_hf_Filippatos_2016.md]
8. Bakris GL, Agarwal R, Chan JC, et al. Effect of finerenone on albuminuria in patients with diabetic nephropathy (ARTS-DN). JAMA. 2015. 📄 [arts_program_Bakris_2015.md]

---
*此檔為主題一之統計深度解讀,撰寫日期基準 2026-07-11。所有具體數字(IC50、Kd、fold、mediation %、HR、CI、NNT、P-interaction)均可 grep 回上列本地全文 MD。統計詮釋(量綱區分、預後 vs 療效修飾、non-inferiority 語意邊界)為延伸解讀;數字未經杜撰。明示邊界:BP-independent 之「獨立」以 SBP 中介 21%、合計未中介約 50% 為界;ARTS/ARTS-HF 之「至少相當」為描述性 surrogate 觀察,非 powered 等效;finerenone 對類固醇型 MRA 的長期硬終點對頭資料本地全無。*
