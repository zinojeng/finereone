# KDIGO 2026 事實 Grep 稽核報告
主文：`06_beyond_t2d_cardiorenal_landscape.md`
來源：`原始PDF/KDIGO_2026_Diabetes_CKD_draft.md`

## 逐項稽核結果

| # | 論斷 | 主文位置 | Grep 結果 | 判定 |
|---|------|---------|-----------|------|
| 1 | Rec 4.4.1（T2D, nsMRA, 1A, "We recommend..."）逐字引述 | L19 | 命中（source L598/L3188），但主文引句省略了 `[≥3 mg/mmol]` 與 `(RASi)` 未加刪節號 | 待議 |
| 2 | eGFR ≥25 ml/min/1.73m²（Rec 4.4.1） | L19 | 命中 | 通過 |
| 3 | UACR ≥30 mg/g（T2D 門檻） | L19, L227 | 命中（source L598等） | 通過 |
| 4 | Practice Point 4.4.2：SGLT2i 與 nsMRA 可同步起始 | L19 | 命中（source L602/L3346） | 通過 |
| 5 | CONFIDENCE：day180 UACR 較 finerenone 多降 29%（LSM ratio 0.71；0.61–0.82） | L19 | 命中逐字（source L3306） | 通過 |
| 6 | CONFIDENCE：較 empagliflozin 多降 32%（0.68；0.59–0.79） | L19 | 命中逐字（source L3306） | 通過 |
| 7 | Practice Point 4.4.3（血鉀監測） | L19 | 命中（source L606/L3350） | 通過 |
| 8 | Practice Point 4.4.4（優先選有腎/CV實證） | L19 | 命中（source L608/L3362）——主文正文提及 4.4.4，但**未列在題目指定條號清單**，仍屬有效補充 | 通過 |
| 9 | Practice Point 4.4.7（不與類固醇型MRA併用） | L19 | 命中（source L614/L3376） | 通過 |
| 10 | 新統合分析：7 studies, nsMRA vs placebo, T2D+CKD | L19 | 命中逐字「7 studies (41 reports)」（source L3290） | 通過 |
| 11 | kidney composite HR 0.84 (0.77–0.92) | L19 | 命中（source L3290） | 通過 |
| 12 | kidney failure HR 0.84 (0.71–0.99) | L19 | 命中（source L3290） | 通過 |
| 13 | HF/HHF HR 0.78 (0.66–0.92) | L19 | 命中（source L3290） | 通過 |
| 14 | all-cause mortality RR 0.90 (0.81–1.00) | L19 | 命中（source L3290） | 通過 |
| 15 | CV mortality RR 0.88 (0.76–1.02) | L19 | 命中（source L3290/3294） | 通過 |
| 16 | nonfatal stroke RR 1.01 (0.83–1.22) | L19 | 命中（source L3294） | 通過 |
| 17 | nonfatal MI RR 0.92 (0.75–1.13) | L19 | 命中（source L3294） | 通過 |
| 18 | 高血鉀 RR 2.09 (1.82–2.39) | L19 | 命中（source L3294） | 通過 |
| 19 | K≥5.5 RR 2.18 (1.98–2.40) | L19 | 命中（source L3294） | 通過 |
| 20 | Figure 19："additional risk-based" 治療、疊加於 foundational therapy 之上 | L19 | 概念命中（source L491, L1674, L493） | 通過 |
| 21 | Rec 4.7.1（T1D, nsMRA, 2C, "We suggest..."）逐字引述 | L39 | 命中（source L771/781/4485/4510），但主文引句同樣省略 `[≥20 mg/mmol]` 未加刪節號 | 待議 |
| 22 | UACR ≥200 mg/g（T1D 門檻） | L39, L97 | 命中 | 通過 |
| 23 | eGFR ≥25 ml/min/1.73m²（Rec 4.7.1） | L39 | 命中 | 通過 |
| 24 | 因 indirectness 作單一 GRADE 降級、僅支持 Level 2 建議 | L39 | 命中逐字（source L4536："single...GRADE downgrade for indirectness"..."Level 2 recommendation"） | 通過 |
| 25 | **T2D 舊版為 2A 級「suggest」（Recommendation 3.8.1）**，本次自 2A 升為 1A | L19, L227 | **未命中**——全文（含全文檢索 "3.8.1"、"2A"、"upgraded"、"previous recommendation" 等）中查無「Recommendation 3.8.1」字樣，亦查無先前版本被標記為「2A」等級之敘述。KDIGO_2026_Diabetes_CKD_draft.md 僅有一句概念性描述（L3192："Since the previous iteration of the guideline, it is the judgment of the Work Group that there is greater availability and familiarity...")，未提供具體舊條號或舊等級數字 | **❌GREP_FAIL（必修）** |
| 26 | 表格列（L97）：KDIGO 2026 草案 Rec 4.7.1（2C）suggest | L97 | 命中 | 通過 |
| 27 | 參考文獻 L227：「Rec 4.4.1...自 2024 版 Rec 3.8.1 之 2A 升級」 | L227 | 同 #25，**未命中** | **❌GREP_FAIL（必修）** |

## 草案標記檢查（KDIGO 2026「公開審查草案／尚未定稿」）
逐一確認四處出現皆有標示：
- L19（段落內文 + 段尾註記「以上均為 KDIGO 2026 公開審查草案 Chapter 4，尚未定稿...」）：✅已標示
- L39（段落內文 + 段尾「該草案 Chapter 4 尚未定稿、內容可能因回饋而改變」）：✅已標示
- L97（表格：「公開審查草案・尚未定稿」）：✅已標示
- L227（參考文獻：「Public Review Draft, March 2026（公開審查草案・尚未定稿...）」）：✅已標示

**草案標記本身：通過，四處皆完整標示，無遺漏。**

---

## 必修項目（❌GREP_FAIL）

### 必修 1：「2A 級」與「Recommendation 3.8.1」為未經來源檔驗證之具體細節
- **位置**：主文 L19（正文）與 L227（參考文獻列表）
- **原文**：
  - L19：「在 KDIGO 2024 / ADA-KDIGO 2022 版本中，T2D 的 nsMRA 為 **2A 級「suggest」(Recommendation 3.8.1)**」
  - L227：「Rec 4.4.1（T2D，nsMRA，*1A*，**自 2024 版 Rec 3.8.1 之 2A 升級**）」
- **問題**：此二處皆將「2A」與「Recommendation 3.8.1」的具體數字/條號標記為引自 `[KDIGO_2026_Diabetes_CKD_draft]`，但對該檔案做全文 grep（含關鍵字 "3.8.1"、"2A"、"upgraded"、"previous recommendation"、"formerly"）均未命中任何相符字串。來源檔中僅有一句不具體的敘述性文字（L3192，"Since the previous iteration of the guideline..."），並未提供舊版的正式條號或正式等級代碼。
- **風險**：這是典型的「confabulated detail」——條號與等級字母級別的精確度看似有出處，實則來源檔內查無此數字，可能是模型外推、錯記，或引用了另一份未列入本次稽核來源清單的文件（如實際的 KDIGO 2024 CPG 全文）。若真有其他出處，應改標為該文件而非 `[KDIGO_2026_Diabetes_CKD_draft]`。
- **建議修正**：
  1. 若能在其他已下載來源（如舊版 KDIGO 2024 CKD-diabetes guideline 全文）中找到「Recommendation 3.8.1」與「2A」字樣，應改標引註來源檔案；
  2. 若找不到可驗證來源，應刪除具體條號「3.8.1」與具體等級「2A」，改為模糊敘述（如：「舊版為較低等級之『suggest』建議」）或直接移除此細節，避免無來源根據之精確數字。

## 待議項目

### 待議 1：Rec 4.4.1 逐字引句省略括號內容未加刪節號
- **位置**：L19
- **原文**：主文以引號包裹「"We recommend adding a nonsteroidal mineralocorticoid receptor antagonist (nsMRA) with proven kidney or cardiovascular benefit for people with T2D, an eGFR ≥25 ml/min per 1.73 m², normal serum potassium concentration, and albuminuria (UACR ≥30 mg/g) while on maximum tolerated dose of RAS inhibitor (1A)"」
- **來源原文**（L598/L3188）：「...albuminuria (UACR ≥30 mg/g **[≥3 mg/mmol]**) while on maximum tolerated dose of RAS inhibitor **(RASi)** (1A).」
- **問題**：主文以直接引號（"..."）呈現「逐字引述」，但實際上悄悄省略了「[≥3 mg/mmol]」與「(RASi)」兩處內容，未使用刪節號（...）標示省略，形式上構成不完全精確的逐字引用。內容本身無誤導性（意義未變），故列為待議而非必修。
- **建議修正**：在省略處補上「...」，或改為非引號式paraphrase。

### 待議 2：Rec 4.7.1 逐字引句同樣省略括號內容
- **位置**：L39
- **原文**：「"...albuminuria (UACR ≥200 mg/g) while on maximum tolerated dose of RASi (2C)"」
- **來源原文**（L771等）：「...albuminuria (UACR ≥200 mg/g **[≥20 mg/mmol]**) while on maximum tolerated dose of RASi (2C).」
- **問題**：同待議1，省略「[≥20 mg/mmol]」未加刪節號。
- **建議修正**：同上。

## 通過項目彙總
- Rec 4.4.1（1A）條號、等級、eGFR/UACR/RASi 門檻：命中
- Practice Points 4.4.2 / 4.4.3 / 4.4.4 / 4.4.7：條號與內容命中
- CONFIDENCE 試驗 UACR 相對降幅與 LSM ratio（29%／0.71［0.61–0.82］；32%／0.68［0.59–0.79］）：逐字命中
- 新統合分析（7 studies）全部 9 組 HR/RR 數值與 95% CI：逐字命中
- Rec 4.7.1（2C）條號、等級、eGFR/UACR/RASi 門檻：命中
- T1D GRADE 單一降級（indirectness）、Level 2 建議：命中
- 四處「公開審查草案／尚未定稿」標示：全數確認存在

## 總結
27 項可查核之具體事實中，25 項通過 grep 驗證，2 項（Rec 4.4.1/4.7.1 逐字引句的括號內容省略未標刪節號）列為待議，**1 組必修**（「2A 級」與「Recommendation 3.8.1」在來源檔中查無依據，共出現於 L19、L227 兩處）。四處「公開審查草案・尚未定稿」警語標示完整、無遺漏。
