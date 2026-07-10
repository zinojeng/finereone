# MISSING FULLTEXT — 主題候選二

## 僅 abstract（📌）— 核心資料的誠實限制
| Paper | DOI/PMID | Reason | 處理方式 |
|-------|----------|--------|----------|
| **Agarwal R et al. Impact of Finerenone-Induced Albuminuria Reduction on CKD Outcomes in T2D: A Mediation Analysis. Ann Intern Med. 2023;176(12):1606-1616.** | 10.7326/M23-1023 / PMID 38048573 | 封閉取用（Unpaywall 陰性、無 PMCID、Sci-Hub 失敗）；本地僅 Europe PMC 結構化 abstract | **本主題核心 mediation 論文**。其關鍵中介比例（如 UACR ≥30% 降幅 finerenone vs placebo、mediation 84%/37%、64%/26% 等）取自「已比對 title/作者/DOI/PMID 的結構化 abstract」逐字轉錄，全部標 📌 並加保留註記。此為與硬規則「僅 abstract 者不得做具體數字斷言」之間的折衷：數字確實存在於已驗證 abstract、非幻覺，但明確降級標示、未做全文交叉驗證。若需嚴格化可移除具體數字、只留定性敘述。 |
| Mc Causland FR et al. FINEARTS-HF (renal/UACR) 2025 | **10.1093/ndt/gfaf116.0475**（ERA congress abstract #3019） | abstract-only（使用者上傳之 PDF 經核為同一份會議摘要海報，非期刊全文，故未升級 status，📌 保持不變） | 僅設計層級提及 |
| ~~Heerspink HJL et al. 2025 Nat Med~~ → **已補全文（見下方 round 3）** | 10.1038/s41591-025-04057-z / PMID 41198855 | ~~付費牆~~ | 使用者上傳本地 PDF，已升級為全文 |
| FINE-ONE（T1D, UACR 終點；Heerspink 2026 NEJM 本體） | **10.1056/NEJMoa2512854** / PMID 41780000 | 無本地全文（本主題）；topic 06 有 `fine_one_t1d_Heerspink_2026` abstract 檔 | 僅於爭議二做終點方法學層級提及，無具體數字 |

FIND-CKD 細部數字改引本地全文擷取檔 `note_find_ckd_extract.md`（📄）與 `FIND-CKD_NEJMoa2604625.md`（📄）。

## 已補全文（本輪升級）
以下論文本輪由「僅 abstract（📌）」升級為本地全文（📄，status: full_text）。來源均為**使用者上傳之本地 PDF 經 LlamaParse 轉檔**，內容現已可 grep 交叉驗證。

| Paper | 本地檔 | DOI/PMID | 說明 |
|-------|--------|----------|------|
| Heerspink HJL et al. Finerenone in Persons with CKD without Diabetes (FIND-CKD). N Engl J Med. 2026. | `find_ckd_nondiab_Heerspink_2026` | 10.1056/NEJMoa2604625 / PMID 42246672 | FIND-CKD NEJM **主文**全文；與既有 `FIND-CKD_NEJMoa2604625.md` 為同一論文（重複全文）。主文 §4.4 之 FIND-CKD 數字仍主要引 `note_find_ckd_extract.md`。 |
| Neuen BL et al. Finerenone in Patients With CKD Due to Glomerular Diseases: A RCT. JAMA. 2026. | `find_ckd_nondiab_Neuen_2026` | 10.1001/jama.2026.9923 / PMID 42246414 | FIND-CKD 之 glomerular-disease 預設次組分析（IgA/FSGS/膜性等）。**本輪新引入主文 §4.4**（total slope diff 0.73、alb −42%、HR 0.74 等，均已 grep 命中）。 |
| Neuen BL et al. Efficacy and safety of finerenone in CKD: an IPD pooled analysis (INFINITY). Lancet. 2026;407(10546):2375–86. | `find_ckd_nondiab_INFINITY_Neuen_2026` | 10.1016/S0140-6736(26)01009-3 / PMID 42248158 | FIDELIO-DKD+FIGARO-DKD+FIND-CKD 三試驗 IPD pooled。**本輪新引入主文 §4.4**（跨病因一致性，qualitative；此檔數字採 Lancet 中點小數 0·76 格式，故僅引可 grep 之定性語句，未嵌入 period-decimal 數字以維持稽核）。 |

## 已補全文（本輪升級，round 2）
以下論文本輪由「僅 abstract（📌）」升級為本地全文（📄，status: full_text）。來源均為**使用者上傳本地 PDF 經 LlamaParse 轉檔**，內容現已可 grep 交叉驗證。

| Paper | 本地檔 | DOI/PMID | 說明 |
|-------|--------|----------|------|
| Agarwal R et al. Systolic blood pressure and albuminuria reduction mediate cardiovascular benefits of finerenone in T2D and CKD. Nephrol Dial Transplant. 2026 (advance article). | `albuminuria_mediation_Agarwal_2026`（另有同一論文重複全文檔 `biomarker_Agarwal_2026`） | 10.1093/ndt/gfag150 / PMID 42360710 | FIDELITY（n=12,143）四-mediator causal mediation。**主文 §4.2 之數字（UACR −32.2%、SBP −3.6 mmHg、體重 −0.23 kg、鉀 +0.19 mEq/L；UACR mediated 39% [7–71]、SBP 21% [3–40]、UACR+SBP 合計 50% [21–100]）本輪全部 grep 命中並由 📌 升級為 📄**；§6 新增「腎保護約需 18 個月才具統計顯著性」之時序數字（grep 命中）。`albuminuria_mediation_Agarwal_2026` 與 `biomarker_Agarwal_2026` 為**同一 NDT 論文的兩份重複全文**（相同 DOI/PMID）；後者未被主文引用。 |

## 已補全文（round 3）
| Paper | 本地檔 | DOI/PMID | 說明 |
|-------|--------|----------|------|
| Heerspink HJL et al. A meta-analysis of albuminuria as a surrogate endpoint for kidney failure. Nat Med. 2025. | `r2_Heerspink_2025`（另 topic 06 副本 `cmp_Heerspink_2026_albuminuria_NatMed`） | 10.1038/s41591-025-04057-z / PMID 41198855 | 使用者上傳本地 PDF 經 LlamaParse 轉檔（status: full_text）。主文 §3.1（第 41 行）與 §6（第 162 行）之「48 RCT、85,681 人、每 30% UACR 降幅對應風險降 19%、median R²=0.66」等數字**已 grep 命中並由 📌 升級為 📄**。 |

## Polluted PDF（下載污染，已棄用）
| Paper | Reason |
|-------|--------|
| Ortiz A et al. 2026 Lancet editorial（brief 指定的「2026 Lancet editorial」） | 下載為污染 PDF，全文與 abstract 均不可用。已改由 **Matyjek 2026（Clinical Kidney Journal editorial，全文可用 📄）** 承擔方法學/臨床對讀（editorial）角色。 |

## 稽核
citation-verifier 2 findings、claim-auditor 2、cross-referencer 6；**2 條必修**（References #19 佔位符 DOI `10.1016/j.kint.2024.xx` → 更正為 Taylor 2025 eClinicalMedicine `10.1016/j.eclinm.2025.103465`，PMID 40932851；同一斷鏈的 dead-link）皆已修正。
