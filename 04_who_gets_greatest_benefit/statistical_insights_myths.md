# 統計迷思與深度解讀 · 主題四（臨床流行病學的統計陷阱）

> 本檔為主題 04「誰得到最大效益」的**統計深度解讀**分冊，鎖定專科醫師在讀 finerenone 次分析時最容易「數字都對、結論卻錯」的五個統計陷阱。每個陷阱用三段式拆解：**❌ 常見誤解 → ✅ 統計正解 → 💡 臨床亮點**。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（只引用摘要已載數字，不對未載內容作斷言）。每個具體數字句末以 `[本地MD檔名]` 標註，供 grep 回溯。LLM 僅負責組織、改寫與**統計詮釋**；詮釋可延伸，數字一律出自本地全文。
>
> **證據分層**：🟢 已確立的統計方法學共識｜🟡 post hoc／探索性／替代終點｜🔴 假說或僅摘要。
>
> **與姊妹檔的分工（勿重複）**：本檔的「經典錨點」——相對風險 vs 絕對風險、「各亞群一致 ≠ 人人同樣受益」、subgroup multiplicity、ICEMAN、risk-based HTE——已在同資料夾 [`methodology_subgroup_relative_vs_absolute.md`](methodology_subgroup_relative_vs_absolute.md) 完整處理。本檔**不重述**那套，只借它當一句話的入口比喻，然後轉向該檔未深入的五個陷阱：**NNT 的三大內在缺陷、ITT vs on-treatment 的選擇偏差、競爭風險、比例風險假設失效、fragility index**。
>
> **經典錨點（一句帶過）**：statin 相對降 29.2% 一致，但 10 年風險 5% 者 ARR 僅 1.5%、50% 者達 14.6%——同一個折扣，省下的絕對金額天差地別。這條「相對恆定 → 絕對放大」的橋樑是全主題的地基（詳見姊妹檔）📄[subgroup_methodology_Sun_2010]。**本檔要問的下一層問題是：當我們把這個絕對受益濃縮成一個叫 NNT 的數字、或用一個單一 HR 概括整段追蹤時，又會踩到哪些坑。**

---

## 迷思一：NNT 是一個「乾淨、可搬運的常數」——NNT 的三大陷阱

NNT（number needed to treat）是床邊最愛用的數字：「治療幾個人可避免一件壞事」。它的親切感恰恰是它最危險的地方——NNT 看起來像一個物理常數，其實是一個**綁定了時間、綁定了族群、還常常藏起信賴區間**的估計值。

### ❌ 常見誤解
「finerenone 腎臟 NNT 大約 60，華人可以低到 7；記住這幾個數字，衛教時直接引用就好。」把 NNT 當成像身高體重一樣可以背、可以跨情境搬運的定值。

### ✅ 統計正解
NNT = 1 / ARR，而 ARR 本身會隨三件事變動，所以 NNT 有三個內建陷阱：

- **(a) 時間依賴——同一群人，不同時點是完全不同的 NNT。** FIDELITY stage 4 CKD 亞群（890 人，占 7%）的 Aalen–Johansen 累積發生率顯示：**腎臟複合終點的 NNT 在第 1 年是 41、第 2 年降到 19、第 3 年變成 −40、第 4 年 −20**（負值即 NNH，代表方向翻轉）📄[pooled_safety_hyperkalemia_Sarafidis_2023]。同一份分析裡，**心血管複合終點的 NNT 卻穩定為 1/2/3/4 年 29/29/31/24**📄[pooled_safety_hyperkalemia_Sarafidis_2023]。一個「NNT ≈ 20」的斷言，不講時點就等於沒講。
- **(b) 信賴區間常被省略，而且可能極寬。** 華人 FIDELIO ≥40% 腎臟終點 NNT **8，但 95% CI 是 4–84**（30 個月，ARR 12.2%，HR 0.59）📄[asian_subgroup_Zhang_2023]；華人 FIGARO ≥40% 終點月 36 NNT **7，95% CI 4–22**📄[asian_subgroup_Li_2025]。點估計 7、8 很誘人，但 CI 上界 22、甚至 84，意思是「真值可能要治療 84 人才防一件事」。報 NNT 不報 CI，是把小樣本的不確定性藏進了一個乾淨數字裡。
- **(c) 不可跨基線風險移植。** FIDELITY 整體心血管 NNT **46（95% CI 29–109）**、整體腎臟 NNT **60（38–142）**📄[stage4_ckd_Agarwal_2022]。這個「平均 NNT」不能套用到高風險華人身上（後者腎臟 NNT 7–12），也不能套用到低風險早期病人身上——因為 ARR 由基線絕對事件率決定，而各族群的基線事件率相差數倍。

### 💡 臨床亮點
NNT 要當「一組帶時間戳與 CI 的區間」來讀，而不是一個記憶點。床邊正確的說法是：「**在像您這樣的高風險（高 UACR、低 eGFR）病人、以 3 年為期，大約每 7 到 12 人可避免一次腎臟惡化事件**」——同時把時間窗、族群、與不確定性一起交代。反過來，看到 stage 4 腎臟 NNT 在第 3 年翻成 NNH，正確反應不是「finerenone 後來有害」，而是「這是 PH 失效 + 競爭風險的產物」（見迷思三、四），單一 NNT 在這裡本就不該被計算。

---

## 迷思二：「on-treatment 分析顯著、ITT 邊緣不顯著，那就用顯著的那個」

### ❌ 常見誤解
Filippatos 2023 的死亡率分析裡，ITT 全因死亡 HR 0.89 只差一點不顯著，但 on-treatment 分析 HR 0.82 顯著了——「既然實際有吃藥的人真的活比較久，就引用 on-treatment 的結果，說 finerenone 降低死亡率」。

### ✅ 統計正解
兩個分析用的是**不同的病人集合**，而 on-treatment 的那個集合不再是隨機化的。具體數字：

- **全因死亡 ITT：HR 0.89（95% CI 0.79–1.00，P = 0.051）**，事件數 finerenone 552 vs placebo 614📄[stage4_ckd_Filippatos_2023]。
- **全因死亡 on-treatment：HR 0.82（95% CI 0.70–0.96，P = 0.014）**，事件數只剩 finerenone 280 vs placebo 344📄[stage4_ckd_Filippatos_2023]。
- 心血管死亡同樣：ITT HR 0.88（0.76–1.02，P = 0.092）→ on-treatment HR 0.82（0.67–0.99，P = 0.040）📄[stage4_ckd_Filippatos_2023]。

關鍵在那組被「蒸發」的事件：全因死亡從 552 掉到 280，超過一半的死亡因為「發生在停藥超過 30 天之後」而被剔除📄[stage4_ckd_Filippatos_2023]。問題是——**會停藥的人往往不是隨機的**：因高血鉀、腎功能惡化、身體變差而停藥者，本來就是預後較差的一群；把他們後續的死亡排除在 finerenone 組之外，等於系統性地替治療組「洗掉」高風險個案，機轉上會**高估**效益、破壞隨機化所保護的可比性。這就是 informative censoring 造成的選擇偏差。作者自己也審慎聲明：ITT 才是隨機對照試驗的主結論，on-treatment 只是輔助視角，並明言不宜過度解讀📄[stage4_ckd_Filippatos_2023]。

### 💡 臨床亮點
對死亡率這個終點，誠實的講法是「**finerenone 顯示降低死亡的趨勢，但 ITT 未達統計顯著（HR 0.89，P = 0.051）**」，不能講成「證實降低死亡率」。可以補一句「在持續服藥者身上效益看似更明顯」，但必須標明這是 on-treatment 觀察、有選擇偏差。真正經得起考驗的硬訊號是猝死——那是在**ITT** 族群就達顯著（HR 0.75，95% CI 0.57–0.996，P = 0.046）📄[stage4_ckd_Filippatos_2023]，這一句才可以放心引用。準則：**當 on-treatment 比 ITT 漂亮時，要警覺不是要慶祝。**

---

## 迷思三：把死亡當成「跟腎衰竭無關的背景雜訊」——競爭風險

### ❌ 常見誤解
算腎臟終點時，把死掉的病人跟失去追蹤（lost to follow-up）一樣「censor 掉」，用標準 Kaplan–Meier 估計腎衰竭的累積發生率——反正他們沒發生腎臟事件嘛。

### ✅ 統計正解
在 CKD + T2D、尤其 stage 4 的病人身上，**死亡與腎衰竭是互相競爭的事件**：一個病人若先死了，他就永遠不可能再進展到透析——死亡不是「還沒發生的腎臟事件」，而是「讓腎臟事件不可能發生」的排他終點。把死亡當獨立設限（censoring）會**高估**腎衰竭的累積發生率，因為 KM 隱含假設「被 censor 的人日後有跟在院者相同的事件率」，而死人的事件率是零。

這正是 FIDELITY 腎臟分析採 **Aalen–Johansen 估計、並明確把全因死亡當作競爭風險**處理的原因——Bakris 2023 與 Sarafidis 2023 都是如此做的📄[stage4_ckd_Bakris_2023]📄[pooled_safety_hyperkalemia_Sarafidis_2023]。統計上有兩種 HR 要分清楚：

- **cause-specific hazard（病因別風險）**：Cox 模型算出的 HR（如腎臟複合 HR 0.77，95% CI 0.67–0.88📄[stage4_ckd_Bakris_2023]），回答「在還活著、還沒腎衰的人裡，finerenone 如何改變下一刻發生腎衰的瞬時風險」——適合談**機轉／生物學效果**。
- **subdistribution hazard（Fine–Gray）**：回答「把死亡的競爭效應算進去後，實際會有多少比例的人累積到腎衰」——適合談**絕對負擔／衛生政策**。

兩者在死亡率高的族群可能給出不同數字，混用會誤導。這也解釋了迷思一裡 stage 4 腎臟 NNT 第 3、4 年翻負的部分成因：晚期病人死亡率高，Aalen–Johansen 下競爭死亡吃掉了後段的腎臟事件空間，讓「腎臟受益」在絕對尺度上被稀釋甚至反轉📄[pooled_safety_hyperkalemia_Sarafidis_2023]。

### 💡 臨床亮點
讀腎臟終點時先問一句：「這個累積發生率有沒有把死亡當競爭風險？」用了 Aalen–Johansen / Fine–Gray 的數字，才是病人實際會經歷的絕對腎衰機率；用天真 KM 的，會系統性高估。對病人溝通時也要誠實：在最晚期的病人身上，finerenone 保住腎臟的「絕對」空間，會被競爭的死亡風險壓縮——這不是藥失效，而是族群的殘酷算術，反而支持「趁 eGFR 還沒掉到 stage 4 就早用」。

---

## 迷思四：一個 HR 就能概括整段追蹤——比例風險假設失效

### ❌ 常見誤解
森林圖上每個終點都有一個 HR 和 CI，直接讀點估計、看 CI 有沒有跨 1 就好。預設「治療效果在整段追蹤期間是同一個固定比例」。

### ✅ 統計正解
Cox 模型與單一 HR 的前提是**比例風險（proportional hazards, PH）假設**：治療對風險的相對效果不隨時間改變。一旦效果隨時間變號，這個假設就失效，硬報一個 HR 會把「前期保護 + 後期反轉」平均成一個誤導的中間值。

FIDELITY stage 4 CKD 腎臟複合終點就是活教材：以 treatment×log(time) 交互檢定，**PH 假設不成立（P < 0.01）**📄[pooled_safety_hyperkalemia_Sarafidis_2023]。作者因此**拒絕報告一個整段的 HR**，改報「**前 2 年 HR 0.63（95% CI 0.42–0.95）**」，並明講：保護效果只出現在頭 2 年，之後方向不一致、精確度隨時間流失（風險差 CI 跨 0 並變寬）📄[pooled_safety_hyperkalemia_Sarafidis_2023]。對應的累積風險差：1 年 −2%（−5 to 0）、2 年 −5%（−10 to −1）、3 年 +3%（−4 to 9）、4 年 +5%（−4 to 14）——一條先降後升的曲線，任何單一 HR 都無法誠實概括📄[pooled_safety_hyperkalemia_Sarafidis_2023]。正因如此，整份 stage 4 分析被明白標為 **exploratory**。

### 💡 臨床亮點
看到「HR at year 2」「landmark analysis」「NC = not calculated because PH not met」這類標註，要立刻意識到：作者是在誠實地告訴你「這個效果會隨時間變」，而不是資料不完整。對 stage 4 病人的正解是「**前 2 年有明確的腎臟保護（HR 0.63），2 年後訊號變不穩定**」，而不是背一個平均 HR。臨床含意反而積極：早期保護真實存在，支持在病人還沒走到最晚期時就介入——晚了，PH 曲線的後半段告訴你效益窗口正在關閉。

---

## 迷思五：P < 0.05 就代表結果穩固——fragility index

### ❌ 常見誤解
「主要終點 P = 0.03，顯著了，證據很強。」把「有沒有跨過 0.05」當成證據強度的開關。

### ✅ 統計正解
**fragility index（FI，脆弱度指數）**問的是另一個問題：要把多少個「沒發生事件」的病人改成「發生事件」，這個顯著結果才會翻回不顯著？FI 越小，結果越脆弱。Zuin 2026 對 finerenone 心血管結果做 fragility 分析（**僅取得摘要 📌**，不擴張細節）：FIDELIO-DKD 主要心血管複合雖然顯著（HR 0.86、**NNT 56**），但 **FI 僅為 4**——只要 4 個病人的結局改變，顯著性就會消失📌[baseline_goals_absolute_Zuin_2026]。相對地，合併後的 FIDELITY（HR 0.86、NNT 59）**FI 達 38**、FIDELITY 的 HF 住院終點（HR 0.78、NNT 91）**FI 23**，屬穩固訊號📌[baseline_goals_absolute_Zuin_2026]。（註：Zuin 2026 fragility 分析僅納入 FIDELIO-DKD、FIGARO-DKD 與 pooled FIDELITY，**未**納入 FINEARTS-HF。）摘要並指出 CV 死亡／MI／中風等單項終點「favourable 但不顯著、reverse FI 低」，屬脆弱📌[baseline_goals_absolute_Zuin_2026]。

### 💡 臨床亮點
FI 給了「顯著」一個質感：單一試驗（FIDELIO，FI 4）的心血管顯著性其實掛在極少數事件上，這正是為什麼**要引用合併分析（FIDELITY，FI 38）而非單一試驗**來支撐心血管論述——這與姊妹檔「整體效果比單一亞群更可靠」的精神一致。因為僅有摘要，本檔只援引其已公開的 FI/NNT 數字，不對方法細節作進一步斷言。

---

## 統計素養檢查表（查房／簡報用一頁）

| 讀到這個時 | 先問這一句 | 對應迷思 |
|---|---|---|
| 一個 NNT 數字 | 哪個時點？CI 多寬？是哪個族群的基線風險？ | 一 |
| on-treatment 比 ITT 漂亮 | 被 censor 掉的事件是不是「非隨機」地偏向高風險者？主結論該用 ITT | 二 |
| 腎臟／硬終點累積發生率 | 有沒有把死亡當競爭風險（Aalen–Johansen / Fine–Gray）？ | 三 |
| 一個概括整段追蹤的 HR | PH 假設成立嗎？有沒有 landmark / 「HR at year 2」的警示？ | 四 |
| 「P < 0.05，顯著」 | fragility index 多少？是單一試驗還是合併分析？ | 五 |
| 任何次分析結論 | 這是拿來「校準判讀」還是被誤用來「改寫適應症」？（見姊妹檔） | 錨點 |

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|---|---|---|
| NNT 時間依賴（stage 4 腎臟 41→19→−40→−20；CV 29/29/31/24） | 🟡 exploratory | `pooled_safety_hyperkalemia_Sarafidis_2023` 📄 |
| NNT 的 CI 極寬（華人腎臟 8〔4–84〕、7〔4–22〕） | 🟡 post hoc | `asian_subgroup_Zhang_2023`、`asian_subgroup_Li_2025` 📄 |
| NNT 不可跨基線風險移植（整體 46 / 60 vs 華人 7–12） | 🟢 方法學 | `stage4_ckd_Agarwal_2022` 📄 |
| ITT（0.89, P=0.051）才是主結論；on-treatment（0.82）有選擇偏差 | 🟢 方法學／🟡 資料 | `stage4_ckd_Filippatos_2023` 📄 |
| 競爭風險：Aalen–Johansen 以死亡為競爭事件；cause-specific vs Fine–Gray | 🟢 方法學 | `stage4_ckd_Bakris_2023`、`pooled_safety_hyperkalemia_Sarafidis_2023` 📄 |
| PH 假設失效（stage 4 腎臟 P<0.01，僅報 2 年 HR 0.63）→ exploratory | 🟡 exploratory | `pooled_safety_hyperkalemia_Sarafidis_2023` 📄 |
| fragility index（FIDELIO FI 4 / NNT 56 vs FIDELITY FI 38） | 🔴 僅摘要 | `baseline_goals_absolute_Zuin_2026` 📌 |
| 相對恆定 → 絕對放大（statin 29.2% → ARR 1.5% vs 14.6%）〔錨點〕 | 🟢 方法學 | `subgroup_methodology_Sun_2010` 📄（詳見姊妹檔） |

---

## 本地全文語料（可 grep 稽核）

📄 全文：`pooled_safety_hyperkalemia_Sarafidis_2023`（FIDELITY stage 4 亞群；NNT 時間序列、PH 失效、Aalen–Johansen 競爭風險——按主題五資料夾，跨主題引用）、`stage4_ckd_Filippatos_2023`（死亡率 ITT vs on-treatment）、`stage4_ckd_Bakris_2023`（腎臟終點、Aalen–Johansen 競爭風險、NNT 60）、`stage4_ckd_Agarwal_2022`（FIDELITY 整體 NNT 46 / 60）、`asian_subgroup_Zhang_2023`（華人 FIDELIO NNT 8〔4–84〕）、`asian_subgroup_Li_2025`（華人 FIGARO NNT 7〔4–22〕）、`subgroup_methodology_Sun_2010`（相對 vs 絕對錨點）。
📌 abstract：`baseline_goals_absolute_Zuin_2026`（fragility index；僅摘要，不擴張細節）。
（相對／絕對、subgroup multiplicity、ICEMAN、risk-based HTE 之完整處理見姊妹檔 `methodology_subgroup_relative_vs_absolute.md`，本檔不重述。）

---

## References（Vancouver 風格，含本地檔）

1. Sarafidis P, Agarwal R, Pitt B, Wanner C, Filippatos G, Boletis J, et al. Outcomes with finerenone in participants with stage 4 CKD and type 2 diabetes: a FIDELITY subgroup analysis. Clin J Am Soc Nephrol. 2023. 📄 [pooled_safety_hyperkalemia_Sarafidis_2023]（主題五資料夾，跨主題引用）
2. Filippatos G, Anker SD, August P, Coats AJS, Januzzi JL, Mankovsky B, et al. Finerenone and effects on mortality in chronic kidney disease and type 2 diabetes: a FIDELITY analysis. Eur Heart J Cardiovasc Pharmacother. 2023;9(2):183–91. 📄 [stage4_ckd_Filippatos_2023]
3. Bakris GL, Ruilope LM, Anker SD, Filippatos G, Pitt B, Rossing P, et al. A prespecified exploratory analysis from FIDELITY examined finerenone use and kidney outcomes. Kidney Int. 2023;103(1):196–206. 📄 [stage4_ckd_Bakris_2023]
4. Agarwal R, Filippatos G, Pitt B, Anker SD, Rossing P, Joseph A, et al. Cardiovascular and kidney outcomes with finerenone: the FIDELITY pooled analysis. Eur Heart J. 2022;43(6):474–84. 📄 [stage4_ckd_Agarwal_2022]
5. Zhang H, Xie J, Hao C, Li X, Zhu D, Zheng H, et al. Finerenone in patients with CKD and type 2 diabetes: the FIDELIO-DKD subgroup from China. Kidney Dis. 2023;9(6):498–506. 📄 [asian_subgroup_Zhang_2023]
6. Li P, Zheng H, Ma J, Lu W, Li L, Liu F, et al. Impact of finerenone on CKD progression in Chinese patients with type 2 diabetes: a FIGARO-DKD subgroup analysis. Front Endocrinol. 2025;16:1568438. 📄 [asian_subgroup_Li_2025]
7. Sun X, Briel M, Walter SD, Guyatt GH. Is a subgroup effect believable? Updating criteria to evaluate the credibility of subgroup analyses. BMJ. 2010;340:c117. 📄 [subgroup_methodology_Sun_2010]
8. Zuin M, Bilato C, Temporelli PL, Oliva F, Savarese G, Metra M, et al. Fragility analysis of cardiovascular outcomes with finerenone in T2D and CKD. Eur J Heart Fail. 2026. 📌 [baseline_goals_absolute_Zuin_2026]（abstract only）

---
*此檔為主題四之統計深度解讀分冊，撰寫日期基準 2026-07-11。所有具體數字均可 grep 回上列本地全文 MD；Zuin 2026 僅取得摘要，其 fragility 方法細節不作進一步斷言。相對／絕對與 subgroup 方法學之完整論述見姊妹檔 `methodology_subgroup_relative_vs_absolute.md`，本檔刻意互補不重複。Sarafidis 2023 全文位於主題五資料夾，為跨主題引用之本地全文。*
