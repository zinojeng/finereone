# Claim Audit — KDIGO 2026 事實 (topic 03: fourth_pillar_or_early_combination)

稽核範圍:主文中所有新加入的 KDIGO 2026 Diabetes/CKD 公開審查草案事實(等級 1A/2C、條號 4.4.1/4.4.2/4.4.3/4.4.7/4.7.1、UACR 門檻、統合分析 HR/RR)。
稽核方法:逐句抽取數字/條號/引號字串,對 `原始PDF/KDIGO_2026_Diabetes_CKD_draft.md` 執行 Grep 逐字比對;並確認每一 KDIGO 2026 段落是否標示「公開審查草案/尚未定稿」。

## 逐項核對結果

| # | 主文位置 | 斷言內容 | Grep 命中(原始PDF行號) | 草案免責聲明是否標示 | Verdict |
|---|---|---|---|---|---|
| 1 | L15 | Recommendation 4.4.1(1A):nsMRA for T2D, eGFR≥25, normal K, UACR≥30 mg/g, on max RASi | L598/L3188 逐字命中 | 段落開頭已載「公開審查草案(僅含 Chapter 1/2/4),尚未定稿、內容可能因回饋而改變」 | 通過 |
| 2 | L15 | Work Group 升級理由:「greater availability and familiarity」+ 多數知情人員會選擇使用 | L3192「greater availability and familiarity with the use of nsMRAs and the majority of well-informed healthcare professionals...would want to receive treatment」;L3316 呼應段落亦同義命中 | 同段已標草案狀態 | 通過 |
| 3 | L15 | 統合分析:7 studies、finerenone 或 esaxerenone vs placebo、T2D+CKD | L3290「7 studies (41 reports)...nsMRA (finerenone or esaxerenone) with placebo」 | 同段 | 通過 |
| 4 | L15 | 腎臟複合終點 HR 0.84(0.77–0.92) | L3290「kidney composite outcome (HR: 0.84; 95% CI: 0.77–0.92)」 | 同段 | 通過 |
| 5 | L15 | kidney failure HR 0.84(0.71–0.99) | L3290/L4047「kidney failure (HR: 0.84; 95% CI: 0.71–0.99)」 | 同段 | 通過 |
| 6 | L15 | HF/HHF HR 0.78(0.66–0.92) | L3290「HF or hospitalizations for HF (HR: 0.78; 95% CI: 0.66–0.92)」 | 同段 | 通過 |
| 7 | L15 | all-cause mortality RR 0.90(0.81–1.00) | L3290/L3294「(RR: 0.90; 95% CI: 0.81–1.00)」 | 同段 | 通過 |
| 8 | L15 | CV mortality RR 0.88(0.76–1.02) | L3290/L3294「cardiovascular mortality (RR: 0.88; 95% CI: 0.76–1.02)」 | 同段 | 通過 |
| 9 | L15 | nonfatal stroke RR 1.01(0.83–1.22) | L3294「stroke (RR: 1.01; 95% CI: 0.83–1.22)」 | 同段 | 通過 |
| 10 | L15 | nonfatal MI RR 0.92(0.75–1.13) | L3294「nonfatal myocardial infarction (RR: 0.92; 95% CI: 0.75–1.13)」 | 同段 | 通過 |
| 11 | L15 | hyperkalemia RR 2.09(1.82–2.39) | L3294「hyperkalemia...RR: 2.09; 95% CI: 1.82–2.39」 | 同段 | 通過 |
| 12 | L15 | K≥5.5 RR 2.18(1.98–2.40) | L3294「serum potassium ≥5.5 mmol/l (RR: 2.18; 95% CI: 1.98–2.40)」 | 同段 | 通過 |
| 13 | L15 | Figure 19「comprehensive strategy」:SGLT2i+RASi+statin = foundational pharmacotherapy;nsMRA+GLP-1RA = additional risk-based pharmacotherapy | L493/L1565「Comprehensive strategy...」;L1624/L1674「foundational pharmacotherapy, additional risk-based pharmacotherapy」;圖說 L491/L1563 列出象限內容一致 | 同段(承接 4.4.1 段落之草案聲明) | 通過 |
| 14 | L15 | T1D 全新 Recommendation 4.7.1(2C):nsMRA for T1D, eGFR≥25, normal K, UACR≥200 mg/g, on max RASi | L771/L781/L4485/L4510 四處逐字命中(含 UACR≥200 mg/g[≥20 mg/mmol]) | 同段 | 通過 |
| 15 | L17 | Practice Point 4.4.2 全文:「For people with T2D treated with RASi who have persistent albuminuria and normal serum potassium, an SGLT2i and nsMRA can be initiated simultaneously」 | L602/L3346 逐字命中 | 該句前綴已標「KDIGO 2026 草案(公開審查草案,尚未定稿)」 | 通過 |
| 16 | L17 | CONFIDENCE 依據數字:combination 較 finerenone 多降 29%(LSMR 0.71;0.61–0.82)、較 empagliflozin 多降 32%(0.68;0.59–0.79) | L3306「29% greater...0.71; 95% CI: 0.61–0.82」及「32% greater...0.68; 95% CI: 0.59–0.79」 | 同段 | 通過 |
| 17 | L17 | 草案明註:「Direct head-to-head comparisons were not available to test nsMRA compared with SGLT2i on composite cardiovascular or kidney outcomes」 | L3304 逐字命中(句尾) | 同段末已重申「(a) 仍屬公開審查草案;(b)...」 | 通過 |
| 18 | L151(take-home #2) | 覆述 4.4.1 升級為 1A、新增 Practice Point 4.4.2 | 同上 L598/L602 | 段內明列「(a) 該文件仍是公開審查草案(2026 年 3 月,僅 Chapter 1/2/4),尚未定稿、可能因回饋而改變;(b)...」 | 通過 |
| 19 | L175(mermaid 圖說) | 覆述 4.4.1(1A)升級與 Practice Point 4.4.2 | 同上 | 「在 KDIGO 2026 公開審查草案(尚未定稿) 中」已標示 | 通過 |
| 20 | L202(參考文獻#22) | 條號清單 4.4.1/4.4.2/4.4.3/4.4.4/4.4.7、Recommendation 4.7.1、Figure 19、Public Review Draft, March 2026 | 4.4.1(L598)、4.4.2(L602)、4.4.3(L606)、4.4.4(L608)、4.4.7(L614)、4.7.1(L771)、Figure 19(L493) 均逐一命中 | 文獻條目本身已寫明「**Public Review Draft, March 2026(公開審查草案,尚未定稿,內容可能因回饋而改變)**」 | 通過 |

## 補充檢查

- **研究設計正確性**:主文將此 7-study 分析正確稱為「統合分析」(meta-analysis),未誤植為 RCT;CONFIDENCE 仍正確標示為其原本的 Phase 2 RCT 設計,未受 KDIGO 2026 段落影響。
- **數字位數**:所有百分比/CI/樣本數(7 studies、41 reports、UACR ≥30 mg/g、UACR ≥200 mg/g、29%/32%、LSMR 0.71/0.68 等)與原文位數完全一致,未見位數膨脹或縮水(confabulated detail)之情形。
- **引號逐字一致性**:主文中以引號直接引用的英文原句(Recommendation 4.4.1 全文、Practice Point 4.4.2 全文、T1D Recommendation 4.7.1 全文、"Direct head-to-head comparisons were not available..."句)與原始 PDF 逐字比對後**完全一致**,僅在極少數地方省略原文括號內的公制單位換算(如 `[≥3 mg/mmol]`、`[≥20 mg/mmol]`),此為可讀性精簡而非竄改,不影響斷言真實性,故不列為必修。
- **草案狀態標示覆蓋率**:檢視全部 6 處引用 KDIGO 2026 草案的段落(L15、L17、L151、L175、L202,以及 L15 段落內部延伸的統合分析與 Figure 19 陳述),均在段落起始或收尾處明確標示「公開審查草案」「尚未定稿」「內容可能因回饋而改變」等字樣,未發現遺漏標示之情形。

## 結論

本次抽核的全部 20 項 KDIGO 2026 具體斷言(條號、等級、UACR 門檻、統合分析 HR/RR、引號原文)均於 `原始PDF/KDIGO_2026_Diabetes_CKD_draft.md` 中 Grep 命中且逐字/數字一致,且每處引用均妥善標示草案未定稿之限制。**未發現 ❌GREP_FAIL 項目,亦未發現漏標草案狀態之情形。**

判定:**全數通過(0 必修、0 待議)**。

---
*本檔案由 claim-auditor(Phase B 三位並行稽核員之一)產出,供 arbitrator 彙整比對。*
