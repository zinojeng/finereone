# Cross-Reference Audit — 03_fourth_pillar_or_early_combination.md

稽核範圍：[檔名] 標記與本地 `原始PDF/*.md` 全文/abstract 逐句核對；序號 range check（引用標記為 `[filename]` 而非 `[N]`，故改核對 References 1–21 與內文標記之對應）；ghost consensus；claim misattribution；synthesis overreach；dead-link；時序檢查。

## 結論摘要
- 所有 `[filename]` 標記在 `原始PDF/` 中皆有對應檔案，**無 dead link**。
- 未發現「許多研究／普遍認為／通常」等 ghost consensus 語言，該類檢查**通過**。
- 時序檢查：所有引用文獻發表年份 ≤2026，主文寫作基準日 2026-07-08，**無未來引用**，通過。
- 主要問題集中在：(a) 將不同分母/不同論文的統計數字合併呈現造成誤導；(b) 將 abstract-only 來源的專屬數字透過錯誤引註「洗白」成有全文查核的引用，違反文件自訂的稽核硬規則；(c) 對 mediation 分析的百分比做誇大解讀（overreach）。

---

## 必修（Must-fix）

### 1. Statin 使用率「>70%」與同一被引來源內部矛盾（misattribution / 數字誤植）
- **原文位置**：第 2.1 節，第 46 行
  > 「…GLP-1RA 使用率 **23%**、statin **>70%**、RASi 近乎 100%」`[confidence_baseline_Agarwal_2025_NDT][confidence_trial_Vaduganathan_2025]`
- **問題**：句中 eGFR、UACR、HbA1c、血鉀、GLP-1RA(23%)、RASi(~100%) 皆為 `confidence_baseline_Agarwal_2025_NDT`（N=801 全體基線）之族群層級數字；唯獨「statin >70%」實際上不存在於該篇——該篇明載 **Statins in 313 (39.1%)**（Table "Medication usage"）。"over 70% use of statins" 一語只出現在 `confidence_trial_Vaduganathan_2025`（KDIGO 風險分層次分析,N=781）的 Discussion 段，且是描述**跨 KDIGO risk category 加總後**的另一種計算方式（各分層分別為 87.5%／74.0%／72.3%），與基線論文的 39.1% 產生**接近 2 倍的落差**，兩篇論文本身即有未解釋的內部不一致。主文未察覺、未標註此矛盾，逕自把「>70%」與其他全族群基線數字並列陳述，讀者對照 `confidence_baseline_Agarwal_2025_NDT` 全文將直接發現矛盾。
- **建議修法**：要嘛拆開兩個數字並各自標注來源與分母（"基線族群 statin 39.1%［baseline 論文］；但依 KDIGO 風險分層之次分析中則為 70%+［Vaduganathan 論文，可能因分層樣本或定義不同］"），要嘛在文中明白註記兩篇論文數字不一致、不可互換使用。

### 2. P=0.91／P=0.85 誤植於 Sinclair editorial，實際來源為未被引用的 abstract-only JACC 論文（misattribution，違反文件自訂稽核規則）
- **原文位置**：第 4 節「爭議(2)」，第 135 行
  > 「CONFIDENCE 的隨機化證據明白顯示：同步起始並未減少 finerenone 介導的高血鉀**(combination vs finerenone 血鉀變化 P=0.91、高血鉀 odds P=0.85 的定性結論見 Sinclair)**」`[hyperkalemia_combo_Sinclair_2026]`
- **問題**：逐字核對 `hyperkalemia_combo_Sinclair_2026.md`（Sinclair & Edmonston editorial 全文），全文**完全沒有出現 P=0.91 或 P=0.85** 這兩個數字；Sinclair 只以文字描述「similar potassium increases and hyperkalemia risk」，未附具體 p 值。這兩個精確 p 值實際出自 `confidence_trial_Agarwal_2026.md`（JACC 高血鉀次分析，📌 **abstract-only**，Ref #6）：「No difference…in mean change in serum potassium (P = 0.91) or the odds of developing hyperkalemia (P = 0.85)」。
  - 這正是文件自身在開頭方法學聲明中明訂的紅線：「凡📌（僅 abstract）之三篇 CONFIDENCE 次分析…其具體數值一律改由已握全文之 editorial 或次級論文交叉引用陳述，未對 abstract 專有數字直接斷言」。本句恰恰把 abstract-only 論文的專屬數字（P=0.91/0.85）直接寫入內文，且**掛在錯誤的引註（Sinclair）之下**，造成「看似有全文查核的引用實際上查無此數字」的假象。
  - 全文逐檔搜尋亦確認 `confidence_trial_Agarwal_2026`（JACC 論文本身）**從未在正文任何 `[filename]` 標記中被引用**——這些數字因此完全遊離於文件自訂的可追溯性規則之外。
- **建議修法**：移除具體 p 值，僅陳述 Sinclair 轉述的定性結論（"無顯著差異"），或改標註為 `[confidence_trial_Agarwal_2026]📌` 並依規則移除具體數字、僅留方向性敘述。

### 3. eGFR mediation 28% 被誇大為「主要由」（Synthesis overreach）
- **原文位置**：第 2.3 節，第 70 行
  > 「更關鍵的是，「把 empagliflozin 加到 finerenone 上」的 UACR 益處**主要由** eGFR 變化中介，而「把 finerenone 加到 empagliflozin 上」的益處則主要是非血流動力學的」`[confidence_egfr_mediation_Agarwal_2026]`
- **問題**：核對 `confidence_egfr_mediation_Agarwal_2026.md`，實際數字為：「acute eGFR change mediated **28%** of the effect of adding empagliflozin to finerenone…but only **5.2%** of the effect when adding finerenone to empagliflozin」。28% 是少數（minority）而非多數中介比例，來源論文自身摘要用語也僅為「**in part** driven by eGFR change」，並未使用「primarily／mainly」。主文把 28% 改寫成「主要由 eGFR 變化中介」，等同把「部分」誇大為「主要」，屬於對統計量做過度延伸的 synthesis overreach，可能誤導讀者以為 empagliflozin-加-在-finerenone-上 這條路徑的血流動力學機轉佔絕對優勢（實際上 72% 仍屬未歸因的其他機轉）。
- **建議修法**：改為「eGFR 變化僅中介其中 28% 的效果（其餘機轉未明），而 finerenone 加在 empagliflozin 上的效果則幾乎不由 eGFR 中介（僅 5.2%，即以非血流動力學路徑為主）」，避免用「主要由」形容 28%。

---

## 待議（Worth discussing）

### 4. FINEARTS-HF 與 FIVE-STAR 之間的矛盾未被揭露（selective synthesis）
- **原文位置**：第 3 節（FINEARTS-HF 段）與第 4 節「爭議(2)」（FIVE-STAR 段）
- **問題**：FINEARTS-HF（`hyperkalemia_combo_Vaduganathan_2025`）顯示：finerenone 使血鉀升高 +0.19 mmol/L，**無論基線是否已慢性使用 SGLT2i 皆相同**（P_interaction=1.00）——即慢性/既有 SGLT2i 背景**沒有**保護作用。但同一節後段（爭議(2)）大幅引用 FIVE-STAR 次分析（經 Sinclair 轉述）主張「已慢性使用 SGLT2i 者，finerenone 誘發血鉀僅升 0.13 vs 未用者 0.37（P_interaction=0.02）」，即慢性 SGLT2i 背景**有**保護作用，並據此建構「SGLT2i 先行、finerenone 後加」的臨床建議流程圖。這兩筆同樣屬於「chronic/pre-existing SGLT2i 背景」的證據方向互相矛盾，但文件僅引用支持其「時序假說」敘事的 FIVE-STAR，未討論 FINEARTS-HF 這筆同樣被引用、卻方向相反的資料如何被調和。這並非數字錯誤，但屬於選擇性綜合（selective synthesis），弱化了第 4 節「時序假說」論證的穩健性。
- **建議修法**：在第 4 節「爭議(2)」補一句誠實揭露："惟需注意，FINEARTS-HF（心衰族群、非糖尿病 CKD 為主）中慢性 SGLT2i 背景並未觀察到相同的血鉀保護效果（P_interaction=1.00），與 FIVE-STAR 的發現方向相反，提示此時序假說可能有族群特異性、仍待驗證"。

### 5. 未被內文引用的孤兒參考文獻（Reference #1）
- **原文位置**：References 列表第 1 條（CONFIDENCE NEJM 主文，Agarwal 2025, doi:10.1056/NEJMoa2410659,📌）
- **問題**：全文以 `grep` 檢索，`[confidence_trial_Agarwal_2025]` 標記**從未在正文任何段落出現**。作為 CONFIDENCE 試驗的主結果論文（也是全文唯一真正的 primary outcome trial report），列在 References #1 卻無對應內文標記，形成孤兒引用（orphan reference）。雖然可以理解是因為其為 abstract-only 而依規則改用次級全文來源（Cheng、Georgianos、Vaduganathan）交叉引用具體數字，但至少應在文中某處以 `[confidence_trial_Agarwal_2025]📌` 標記其定性存在（如試驗結論本身），而非完全不掛標記。
- **建議修法**：在第 2.2 節首次提及 CONFIDENCE 主要結果處，補上 `[confidence_trial_Agarwal_2025]` 標記（僅作定性佐證、不引其獨有數字），使 References #1 不再是孤兒引用。

### 6. Singh 2026（FIDELITY 三藥）之 eGFR slope 益處「都存在」掩蓋了不顯著的次分組
- **原文位置**：第 2.3 節，第 70 行
  > 「此方向與 FIDELITY-Singh 全文一致：finerenone 對 UACR 與 eGFR slope 的益處在有無 SGLT2i / GLP-1RA 下都存在，佐證其為獨立於 SGLT2i 血流動力學之外的第二條機轉」`[hyperkalemia_combo_Singh_2026]`
- **問題**：核對原文，chronic eGFR slope 的 finerenone-vs-placebo 治療差異在「無 SGLT2i/GLP-1RA」「SGLT2i-only」「GLP-1RA-only」三個次族群皆達統計顯著（P<0.04），但在「合併 SGLT2i+GLP-1RA」（三藥）次族群中 **P=0.089，未達統計顯著**（LS-mean 治療差異 1.19，95% CI −0.18 至 2.56，跨零）。主文用「都存在」一詞抹平了這個關鍵的不顯著結果，略為誇大了 finerenone 在三藥背景下 eGFR-slope 效益的確定性。
- **建議修法**：加註「惟在合併 SGLT2i+GLP-1RA 的三藥次族群中，此差異未達統計顯著（P=0.089），可能反映樣本數過小（n=167）」。

### 7. GLP-1RA「對心衰幾乎不提供保護」與同文引用的 Neuen 數據存在張力（未經調和的內部矛盾）
- **原文位置**：第 1.2 節，第 22 行
  > 「GLP-1RA 主要補的是動脈粥狀硬化事件(MI 降約 11%)，對心衰**幾乎不提供保護**——這與 SGLT2i/finerenone 形成鮮明對比」`[r2_Agarwal_2023]`
- **問題**：此句精確轉述 `r2_Agarwal_2023`（Agarwal & Fouque 2023 editorial）原文「No protection from heart failure is seen with these agents」，故對照該來源本身是**準確**的（非誤引）。但同一份主文在下一段（第 23 行）緊接著引用 `glp1_cardiorenal_Neuen_2024` 的資料，其中 GLP-1RA 單獨對 HHF 的估計效果為 **HR 0.89（95% CI 0.82–0.98）**——這是統計上顯著的 11% 相對風險下降，而非「幾乎不提供保護」。兩份被同一文件引用之來源（2023 editorial vs. 2024 跨試驗 actuarial 分析）對 GLP-1RA 心衰保護力的定性描述互相矛盾，主文未點出兩者的落差，讀者可能誤以為 GLP-1RA 對心衰完全無效，但表 3 與內文的整體分工論述又引用了指向「有一定效果、但遠不如另兩支柱」的數字。
- **建議修法**：將「幾乎不提供保護」軟化為「保護效果遠弱於 SGLT2i/finerenone（Neuen 2024 估計 HR 0.89 vs 0.64／0.78）」，並同時標註兩個來源，避免二元對立的措辭掩蓋 Neuen 的顯著（雖然較小）效果量。

---

## 通過（Pass）
- Dead-link / 序號範圍檢查：全部 `[filename]` 標記皆存在對應本地檔案；References #1–21 與內文標記的一對一對應關係經核對一致（除上述孤兒引用 #1 外）。
- Ghost consensus 語言檢查：未檢出「許多研究／多數證據／普遍認為／通常」等未經量化引用支撐的模糊斷言。
- 時序檢查（temporal anachronism）：全部引用文獻發表年份 ≤2026（主文基準日 2026-07-08），無未來引用。
- 大量具體數字（FIDELITY HR/CI、CONFIDENCE UACR/eGFR/血鉀、Wen/Muhammad 統合分析 OR/RR、Neuen lifetime model、Rossing FIDELITY-SGLT2i 交互作用、KDIGO 2024 建議等級與三項證據缺口）逐一與本地全文核對後**均準確**，未發現額外的 misattribution 或捏造引用。

---

*稽核完成，已通知 arbitrator。*
