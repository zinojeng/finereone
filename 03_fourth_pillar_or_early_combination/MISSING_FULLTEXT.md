# MISSING FULLTEXT — 主題候選三

## 僅 abstract（📌）— 其專有數字改由全文次級來源交叉引用,未直接斷言
| Paper | 內容 | Reason | 處理方式 |
|-------|------|--------|----------|
| `confidence_trial_Agarwal_2025`（NEJM CONFIDENCE 主文） | Day 180 UACR 52%/29%/32% | NEJM 付費牆,僅 Europe PMC abstract metadata | 52%/29%/32% 等數字改由全文 Cheng 2025、Georgianos 2025、Vaduganathan 2025、Singh 2026 引述佐證 |
| `confidence_egfr_mediation_Agarwal_2026`（JASN, eGFR mediation） | eGFR-mediated fraction 28% / 5.2% | abstract only | 中介比例（28%、5.2%）取自結構化 abstract 逐字（grep 可回),定性結論交叉佐證 |
| `confidence_trial_Agarwal_2026`（JACC 高血鉀） | 15.3% vs 18.6%；P=0.91/0.85 | abstract only | 專有 P 值不直接斷言;定性結論由 Sinclair editorial 轉述,15.3% vs 18.6% 由 Cheng 全文引用 |

## brief 提及但本地無對應全文者（未虛構引用）
- **NEJM editorial《Combination Therapy for CKD and Diabetes》**：不在本地檔案清單中，未虛構引用。其「正方」論述角色改由已握全文的 **Georgianos 2025（Diabetes Obes Metab）** 與 **Cheng 2025（Diabetes Ther）** editorial 承擔。

## anti-pollution 機制正常運作
多個 fetch 於 fallback chain 取回不相干的 polluted PDF，已依協定丟棄，僅保留 publisher-provided abstract（檔內留有 provenance 註記）。無污染內容進入語料庫。

## 稽核
citation-verifier 4 / claim-auditor 5 / cross-referencer 7 findings；**5 條必修全部修正**（grep-verified）：References #12 補正確 DOI（BMC Nephrol 10.1186/s12882-025-04710-2）;移除 JACC abstract-only 專有 P 值改定性轉述;statin 比例拆分分母差異（39.1% 全群 vs Vaduganathan per-risk-layer >70%);eGFR mediation「主要由」→ 精確 28%/5.2%。
