# MISSING FULLTEXT — 主題候選三

## 僅 abstract（📌）— 其專有數字改由全文次級來源交叉引用,未直接斷言
| Paper | 內容 | Reason | 處理方式 |
|-------|------|--------|----------|
| `confidence_trial_Agarwal_2025`（NEJM CONFIDENCE 主文） | Day 180 UACR 52%/29%/32% | NEJM 付費牆,僅 Europe PMC abstract metadata | 52%/29%/32% 等數字改由全文 Cheng 2025、Georgianos 2025、Vaduganathan 2025、Singh 2026 引述佐證 |
| `confidence_egfr_mediation_Agarwal_2026`（JASN, eGFR mediation） | eGFR-mediated fraction 28% / 5.2% | abstract only | 中介比例（28%、5.2%）取自結構化 abstract 逐字（grep 可回),定性結論交叉佐證 |
| `confidence_trial_Agarwal_2026`（JACC 高血鉀） | 15.3% vs 18.6%；P=0.91/0.85 | abstract only | 專有 P 值不直接斷言;定性結論由 Sinclair editorial 轉述,15.3% vs 18.6% 由 Cheng 全文引用 |

## 已補全文（本輪升級）
本輪由使用者上傳本地 PDF、經 LlamaParse 轉為 Markdown 而新增之全文（先前本主題無此獨立檔）：

| Paper | 檔名 | 內容 | 來源 |
|-------|------|------|------|
| Rossing 2022（FIDELITY × SGLT2i subgroup, Diabetes Care 2022;45(12):2991–2998; doi:10.2337/dc22-0294） | `原始PDF/sglt2i_subgroup_FIDELITY_Rossing_2022.md` | 完整全文含 Table 1（基線特徵）、Table 2（安全性）、Figure 1（CV/腎/HHF/死亡 HR 與 P_interaction）、eGFR slope 與 UACR 分層數字，皆可 grep | 使用者本地上傳 PDF（Agarwal 2022 dc220294.pdf）經 LlamaParse 轉檔，status: full_text |

說明：本主題原已握有同一論文之 PMC 全文次級檔 `hyperkalemia_combo_Rossing_2022.md`（PMC9862372，content_verified），主文既有 FIDELITY 引用維持不變；新檔提供更完整之基線表（Table 1）與安全性表（Table 2）逐字數字，供 confounding-by-indication 量化佐證。本輪據此於主文第 3 節之「證據層級誠實標示」補入一處 grep 驗證數字（基線 eGFR 66.3 vs 57.0、UACR 448 vs 521、GLP-1RA 19.0% vs 6.4%），標 📄[sglt2i_subgroup_FIDELITY_Rossing_2022]。

（註：下表三篇 CONFIDENCE 次分析仍為 abstract-only 📌，本輪未升級、標記不變。）

## brief 提及但本地無對應全文者（未虛構引用）
- **NEJM editorial《Combination Therapy for CKD and Diabetes》**：不在本地檔案清單中，未虛構引用。其「正方」論述角色改由已握全文的 **Georgianos 2025（Diabetes Obes Metab）** 與 **Cheng 2025（Diabetes Ther）** editorial 承擔。

## anti-pollution 機制正常運作
多個 fetch 於 fallback chain 取回不相干的 polluted PDF，已依協定丟棄，僅保留 publisher-provided abstract（檔內留有 provenance 註記）。無污染內容進入語料庫。

## 稽核
citation-verifier 4 / claim-auditor 5 / cross-referencer 7 findings；**5 條必修全部修正**（grep-verified）：References #12 補正確 DOI（BMC Nephrol 10.1186/s12882-025-04710-2）;移除 JACC abstract-only 專有 P 值改定性轉述;statin 比例拆分分母差異（39.1% 全群 vs Vaduganathan per-risk-layer >70%);eGFR mediation「主要由」→ 精確 28%/5.2%。
