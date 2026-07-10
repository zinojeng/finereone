# Claim Audit — 主題05：高血鉀與 eGFR dip 安全工程學
## 範圍：新加入的 KDIGO 2026 事實（等級 1A/2C、條號 4.4.1/4.4.2/4.4.3/4.4.7/4.7.1、UACR 門檻、統合分析 HR/RR）

稽核方法：對 `05_hyperkalemia_egfr_dip_safety_engineering.md` 中每個標註 `[KDIGO_2026_Diabetes_CKD_draft]` 的句子，逐一到
`原始PDF/KDIGO_2026_Diabetes_CKD_draft.md` 執行 Grep 比對數字、條號、引號字串，並確認「公開審查草案／尚未定稿」標示存在。

---

## 逐項比對結果

| # | 主文位置 | 論斷 | Grep 結果 | 草案標示 | Severity |
|---|---|---|---|---|---|
| 1 | L25 | Recommendation 4.4.1（1A），T2D、eGFR ≥25、血鉀正常、UACR ≥30 mg/g、最大耐受 RASi 上 | ✅ 命中 L598/L3188（條號、等級、門檻數字全部一致） | ✅（本段起首即標「公開審查草案（尚未定稿）」，段末重複標示） | 通過 |
| 2 | L25 | 直接引號「We recommend adding a nonsteroidal mineralocorticoid receptor antagonist (nsMRA) with proven kidney or cardiovascular benefit for people with T2D, an eGFR ≥25 ml/min per 1.73 m², normal serum potassium concentration, and albuminuria (UACR ≥30 mg/g) while on maximum tolerated dose of RAS inhibitor (1A)」 | ⚠️ 部分命中：原文為 `...albuminuria (UACR ≥30 mg/g **[≥3 mg/mmol]**) while on maximum tolerated dose of RAS inhibitor (RASi) (1A)`。主文引號內文字**省略了 `[≥3 mg/mmol]`（mmol/L 單位換算）與 `(RASi)` 縮寫展開**，內容未變造但非逐字引用 | ✅ | **待議**（引號逐字性瑕疵，非事實錯誤——建議補回省略片段或改用刪節號） |
| 3 | L25 | 升級理由：Work Group 判斷 nsMRA「可用性與熟悉度提高」，多數知情醫療人員與病人會選擇使用、僅少數不會 | ✅ 命中 L3192（"greater availability and familiarity with the use of nsMRAs...majority of well-informed healthcare professionals and people with T2D and CKD...would want to receive treatment with an nsMRA, while only a small proportion..."） | ✅ | 通過 |
| 4 | L27 | Practice Point 4.4.3 引號「To mitigate risk of hyperkalemia, select people with consistently normal serum potassium concentration and monitor serum potassium regularly after initiation of an nsMRA」 | ✅ 逐字命中 L606/L3350 | ✅ | 通過 |
| 5 | L27 | K⁺ ≤4.8 mmol/L 為試驗篩選閾值；FDA label 血鉀 >5.0 mmol/L 不得起始；多數高血鉀事件可用「暫停 72 小時」處理 | ✅ 命中 L3324（"4.8 mmol/l was the threshold at screening...FDA label, serum potassium should not be >5 mmol/l...treatment pauses of 72 hours"） | ✅ | 通過 |
| 6 | L27 | Practice Point 4.4.7 引號「Do not use steroidal and nsMRA concurrently」 | ✅ 逐字命中 L614/L3376 | ✅ | 通過 |
| 7 | L69 | 新統合分析：7 studies、nsMRA(finerenone/esaxerenone) vs placebo、T2D+CKD | ✅ 命中 L3290（"a total of 7 studies (41 reports)...compared an nsMRA (finerenone or esaxerenone) with placebo"） | ✅ | 通過 |
| 8 | L69 | hyperkalemia（未細分）RR 2.09（95% CI 1.82–2.39） | ✅ 逐字命中 L3294 | ✅ | 通過 |
| 9 | L69 | K⁺ ≥5.5 mmol/L RR 2.18（95% CI 1.98–2.40） | ✅ 逐字命中 L3294 | ✅ | 通過 |
| 10 | L69 | 腎複合終點 HR 0.84（0.77–0.92） | ✅ 逐字命中 L3290 | ✅ | 通過 |
| 11 | L69 | kidney failure HR 0.84（0.71–0.99） | ✅ 逐字命中 L3290 | ✅ | 通過 |
| 12 | L69 | HF/HHF HR 0.78（0.66–0.92） | ✅ 逐字命中 L3290 | ✅ | 通過 |
| 13 | L89 | Practice Point 4.4.2 引號「For people with T2D treated with RASi who have persistent albuminuria and normal serum potassium, an SGLT2i and nsMRA can be initiated simultaneously」 | ✅ 逐字命中 L602/L3346 | ✅ | 通過 |
| 14 | L89 | CONFIDENCE：combo vs finerenone UACR 降幅多 29%（LSM ratio 0.71；0.61–0.82）；vs empagliflozin 多 32%（0.68；0.59–0.79） | ✅ 逐字命中 L3306 | ✅ | 通過 |
| 15 | L89 | 引號「both safe and effective」 | ✅ 逐字命中 L3304（"combination therapy comprising these agents is both safe and effective (Practice Point 4.4.2)"） | ✅ | 通過 |
| 16 | L206/249/250/258 | Recommendation 4.4.1 由 2A 升為 1A；新增 Practice Point 4.4.2（同步起始） | ✅ 條號、等級皆與來源一致 | ✅（各處均標「尚未定稿」／「公開審查草案」） | 通過 |
| 17 | L250 | 首度納入 T1D 建議 Recommendation 4.7.1（2C） | ✅ 逐字命中 L771/L781（"Recommendation 4.7.1: We suggest adding an nsMRA...(2C)"），為 T2D 章節外新增之 T1D 建議 | ✅ | 通過 |
| 18 | L275（參考文獻） | 「Public Review Draft, March 2026」 | ✅ 命中來源文件封面（L5–8：`### PUBLIC REVIEW DRAFT` / `### MARCH 2026`），另 L10 明載"This is a draft document shared for public review and feedback only. The content of this draft will change based on the feedback received..." | ✅ | 通過 |
| 19 | L275 | 參考文獻列出之條號、RR/HR 統計彙總（4.4.1/4.4.2/4.4.3/4.4.7/4.7.1、RR 2.09/2.18） | ✅ 與各條號原文逐一核對一致 | ✅ | 通過 |

---

## 必修（Grep 不到 或 未標草案）

**無**。所有帶 `[KDIGO_2026_Diabetes_CKD_draft]` 標籤的條號、等級、UACR/eGFR 門檻、RR/HR 統計數字，經逐一 Grep 均命中原始草案文字，且每一處引用段落均有「公開審查草案／尚未定稿」明示（含正文與參考文獻條目）。

## 待議

- **L25 引號瑕疵**：Recommendation 4.4.1 全文引號省略了原文括號內的 `[≥3 mg/mmol]`（UACR 單位換算）與 `(RASi)` 縮寫展開。內容實質未變造（數字、條號、等級皆正確），但依「引號內字串逐字一致」的稽核標準不算完全逐字引用。建議修正為完整引號或改寫為間接敘述以符合引用規範。

## 通過

- 條號核對：4.4.1／4.4.2／4.4.3／4.4.7／4.7.1 全部確認存在於草案且與正文引用的內容（等級、人群、門檻）一致。
- 統合分析數字核對：hyperkalemia RR 2.09（1.82–2.39）、K≥5.5 RR 2.18（1.98–2.40）、腎複合 HR 0.84（0.77–0.92）、kidney failure HR 0.84（0.71–0.99）、HF/HHF HR 0.78（0.66–0.92）、7 studies，全部逐字命中。
- CONFIDENCE 數字核對：29%/32%、LSM ratio 0.71（0.61–0.82）／0.68（0.59–0.79），逐字命中。
- 「公開審查草案／尚未定稿」標示：全文 9 處提及 KDIGO 2026 事實的段落（L13、L21、L25、L27、L69、L89、L206、L249、L250、L258、L275）均有標示，無漏標情形。
- 研究設計檢查：本主題無 RCT/cohort 混淆問題——KDIGO 2026 統合分析明確描述為 7 篇研究之 meta-analysis（非單一 RCT 稱謂），主文亦未誤稱為 RCT。

---

**通知**：本稽核已完成，結果請 arbitrator 彙整。核心結論——KDIGO 2026 相關新事實在事實準確性與草案標示上全數通過，僅 1 處引號逐字性瑕疵列為待議（不影響事實正確性）。
