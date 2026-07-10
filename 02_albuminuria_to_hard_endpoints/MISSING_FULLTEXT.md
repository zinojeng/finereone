# MISSING FULLTEXT — 主題候選二

## 僅 abstract（📌）— 核心資料的誠實限制
| Paper | DOI/PMID | Reason | 處理方式 |
|-------|----------|--------|----------|
| **Agarwal R et al. Impact of Finerenone-Induced Albuminuria Reduction on CKD Outcomes in T2D: A Mediation Analysis. Ann Intern Med. 2023;176(12):1606-1616.** | 10.7326/M23-1023 / PMID 38048573 | 封閉取用（Unpaywall 陰性、無 PMCID、Sci-Hub 失敗）；本地僅 Europe PMC 結構化 abstract | **本主題核心 mediation 論文**。其關鍵中介比例（如 UACR ≥30% 降幅 finerenone vs placebo、mediation 84%/37%、64%/26% 等）取自「已比對 title/作者/DOI/PMID 的結構化 abstract」逐字轉錄，全部標 📌 並加保留註記。此為與硬規則「僅 abstract 者不得做具體數字斷言」之間的折衷：數字確實存在於已驗證 abstract、非幻覺，但明確降級標示、未做全文交叉驗證。若需嚴格化可移除具體數字、只留定性敘述。 |
| Agarwal R et al. 2026 (NDT) | — | abstract-only / 付費牆 | 僅設計/背景引用 |
| Mc Causland FR et al. FINEARTS-HF (renal/UACR) 2025 | — | abstract-only | 僅設計層級提及 |
| Heerspink HJL et al. 2025 Nat Med | — | 付費牆 | 未做具體數字斷言 |
| FINE-ONE（T1D, UACR 終點） | — | 無本地全文 | 僅於爭議二做終點方法學層級提及，無具體數字 |

FIND-CKD 細部數字改引本地全文擷取檔 `note_find_ckd_extract.md`（📄）與 `FIND-CKD_NEJMoa2604625.md`（📄）。

## 已補全文（本輪升級）
以下論文本輪由「僅 abstract（📌）」升級為本地全文（📄，status: full_text）。來源均為**使用者上傳之本地 PDF 經 LlamaParse 轉檔**，內容現已可 grep 交叉驗證。

| Paper | 本地檔 | DOI/PMID | 說明 |
|-------|--------|----------|------|
| Heerspink HJL et al. Finerenone in Persons with CKD without Diabetes (FIND-CKD). N Engl J Med. 2026. | `find_ckd_nondiab_Heerspink_2026` | 10.1056/NEJMoa2604625 / PMID 42246672 | FIND-CKD NEJM **主文**全文；與既有 `FIND-CKD_NEJMoa2604625.md` 為同一論文（重複全文）。主文 §4.4 之 FIND-CKD 數字仍主要引 `note_find_ckd_extract.md`。 |
| Neuen BL et al. Finerenone in Patients With CKD Due to Glomerular Diseases: A RCT. JAMA. 2026. | `find_ckd_nondiab_Neuen_2026` | 10.1001/jama.2026.9923 / PMID 42246414 | FIND-CKD 之 glomerular-disease 預設次組分析（IgA/FSGS/膜性等）。**本輪新引入主文 §4.4**（total slope diff 0.73、alb −42%、HR 0.74 等，均已 grep 命中）。 |
| Neuen BL et al. Efficacy and safety of finerenone in CKD: an IPD pooled analysis (INFINITY). Lancet. 2026;407(10546):2375–86. | `find_ckd_nondiab_INFINITY_Neuen_2026` | 10.1016/S0140-6736(26)01009-3 / PMID 42248158 | FIDELIO-DKD+FIGARO-DKD+FIND-CKD 三試驗 IPD pooled。**本輪新引入主文 §4.4**（跨病因一致性，qualitative；此檔數字採 Lancet 中點小數 0·76 格式，故僅引可 grep 之定性語句，未嵌入 period-decimal 數字以維持稽核）。 |

## Polluted PDF（下載污染，已棄用）
| Paper | Reason |
|-------|--------|
| Ortiz A et al. 2026 Lancet editorial（brief 指定的「2026 Lancet editorial」） | 下載為污染 PDF，全文與 abstract 均不可用。已改由 **Matyjek 2026（Clinical Kidney Journal editorial，全文可用 📄）** 承擔方法學/臨床對讀（editorial）角色。 |

## 稽核
citation-verifier 2 findings、claim-auditor 2、cross-referencer 6；**2 條必修**（References #19 佔位符 DOI `10.1016/j.kint.2024.xx` → 更正為 Taylor 2025 eClinicalMedicine `10.1016/j.eclinm.2025.103465`，PMID 40932851；同一斷鏈的 dead-link）皆已修正。
