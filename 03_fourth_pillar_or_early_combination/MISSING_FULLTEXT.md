# MISSING FULLTEXT — 主題候選三

## 僅 abstract（📌）— 其專有數字改由全文次級來源交叉引用,未直接斷言
| Paper | DOI / PMID | 內容 | Reason | 處理方式 |
|-------|-----------|------|--------|----------|
| （本輪三篇 CONFIDENCE 次分析已全部升級為本地全文,見下方「已補全文（本輪升級,round 2）」小節） | — | — | — | — |

## 已補全文（本輪升級）
本輪由使用者上傳本地 PDF、經 LlamaParse 轉為 Markdown 而新增之全文（先前本主題無此獨立檔）：

| Paper | 檔名 | 內容 | 來源 |
|-------|------|------|------|
| Rossing 2022（FIDELITY × SGLT2i subgroup, Diabetes Care 2022;45(12):2991–2998; doi:10.2337/dc22-0294） | `原始PDF/sglt2i_subgroup_FIDELITY_Rossing_2022.md` | 完整全文含 Table 1（基線特徵）、Table 2（安全性）、Figure 1（CV/腎/HHF/死亡 HR 與 P_interaction）、eGFR slope 與 UACR 分層數字，皆可 grep | 使用者本地上傳 PDF（Agarwal 2022 dc220294.pdf）經 LlamaParse 轉檔，status: full_text |

說明：本主題原已握有同一論文之 PMC 全文次級檔 `hyperkalemia_combo_Rossing_2022.md`（PMC9862372，content_verified），主文既有 FIDELITY 引用維持不變；新檔提供更完整之基線表（Table 1）與安全性表（Table 2）逐字數字，供 confounding-by-indication 量化佐證。本輪據此於主文第 3 節之「證據層級誠實標示」補入一處 grep 驗證數字（基線 eGFR 66.3 vs 57.0、UACR 448 vs 521、GLP-1RA 19.0% vs 6.4%），標 📄[sglt2i_subgroup_FIDELITY_Rossing_2022]。

## 已補全文（本輪升級,round 2）
以下三篇 CONFIDENCE 次分析（及 FINEARTS-HF 本體）由使用者上傳本地 PDF、經 LlamaParse 轉為 Markdown，`status: full_text`，內容現可 grep，主文 📌 已改標 📄：

| Paper | 檔名 | DOI / PMID | grep 驗證之被引數字 | 來源 |
|-------|------|-----------|--------------------|------|
| Agarwal 2025（NEJM CONFIDENCE 主文） | `原始PDF/confidence_trial_Agarwal_2025.md` | 10.1056/NEJMoa2410659 / PMID 40470996 | Day 180 UACR −52%（combination）、−32%（fine）、−29%（empa）;組間 LSMR 0.71（0.61–0.82）、0.68（0.59–0.79） | 使用者上傳本地 PDF 經 LlamaParse 轉檔 |
| Agarwal 2026（JASN, eGFR mediation） | `原始PDF/confidence_egfr_mediation_Agarwal_2026.md` | 10.1681/ASN.0000001071 / PMID 41905767 | percent mediated 28%（加 empa 於 fine）、5.2%（加 fine 於 empa） | 使用者上傳本地 PDF 經 LlamaParse 轉檔 |
| Agarwal 2026（JACC 高血鉀） | `原始PDF/confidence_trial_Agarwal_2026.md` | 10.1016/j.jacc.2025.10.049 / PMID 41493296 | 血鉀平均變化 P = 0.91、高血鉀 odds P = 0.85（combination vs finerenone 均無顯著差異） | 使用者上傳本地 PDF 經 LlamaParse 轉檔 |
| Solomon 2024（FINEARTS-HF NEJM 本體） | `原始PDF/r2_Solomon_2024.md` | — | `status: full_text`;本主題主文未直接 bracket 引用此檔（FINEARTS-HF 相關數字現由 `hyperkalemia_combo_Vaduganathan_2025` 承擔），故無 📌→📄 變更 | 使用者上傳本地 PDF 經 LlamaParse 轉檔 |

註（JACC 數字對照）：主文第 2.4 節「combination 15.3% vs finerenone 單藥 18.6%」係由 **Cheng 2025 全文**（`combination_editorial_Cheng_2025.md`,grep 命中）引 CONFIDENCE 之數字,予以保留;JACC 全文本身以「at-risk 分母」報 40/265（15.1%）vs 48/255（18.8%）——兩者為不同分母之表述,主文既有數字仍正確歸因於 Cheng,不改動。

## brief 提及但本地無對應全文者（未虛構引用）
- **NEJM editorial《Combination Therapy for CKD and Diabetes》**：不在本地檔案清單中，未虛構引用。其「正方」論述角色改由已握全文的 **Georgianos 2025（Diabetes Obes Metab）** 與 **Cheng 2025（Diabetes Ther）** editorial 承擔。

## anti-pollution 機制正常運作
多個 fetch 於 fallback chain 取回不相干的 polluted PDF，已依協定丟棄，僅保留 publisher-provided abstract（檔內留有 provenance 註記）。無污染內容進入語料庫。

## 稽核
citation-verifier 4 / claim-auditor 5 / cross-referencer 7 findings；**5 條必修全部修正**（grep-verified）：References #12 補正確 DOI（BMC Nephrol 10.1186/s12882-025-04710-2）;移除 JACC abstract-only 專有 P 值改定性轉述;statin 比例拆分分母差異（39.1% 全群 vs Vaduganathan per-risk-layer >70%);eGFR mediation「主要由」→ 精確 28%/5.2%。
