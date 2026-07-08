# MISSING FULLTEXT — 主題候選五

主文 20 篇引用**全部 📄（本地全文，grep 可驗）**。以下為資料夾內存在但本輪未讀取內文/未引用者，以維持「全文可追溯」原則。

## 未讀取內文 → 未引用（避免自創數字）
| Paper | 處理 |
|-------|------|
| `egfr_dip_reversibility_Oh_2026`（RAAS 因果 eGFR）、`r2_Holtkamp_2011`（losartan eGFR dip 預後） | 資料夾有檔但未讀內文;eGFR dip 預後論點改以已讀之 Ku 2024、Matsumoto 2025 支撐 |
| `pooled_safety_hyperkalemia_Bakris_2020`（FIDELIO 主文） | 未讀全文;FIDELIO 安全數字改由已核實的 Agarwal 2022 與 EMA/FDA label 提供 |
| CONFIDENCE 主結果（NEJM Agarwal 2025, NEJMoa2410659） | 本地無全文;combination vs 單藥高血鉀改用已讀之 Vaduganathan 2025（NDT）Table 2 與 Agarwal 2025（GLP-1 次分析）實際數字 |
| abstract-only 檔（Neuen_2026、Mentz_2025、Oshima_2021 等） | 未使用 |

## fetch 失敗（內容過濾）
| Paper | Reason |
|-------|--------|
| potassium binder Agarwal | workflow fetch agent 遭 content-filtering 攔下（`Output blocked by content filtering policy`）。potassium binder 論點改由已取得全文 AMBER / DIAMOND / EMCREG 支撐 |

## 稽核
citation-verifier 7 / claim-auditor 2 / cross-referencer 6；**1 條必修（ghost consensus）**已修正:§3.4 移除「與 SGLT2i 一貫降低高血鉀的 meta 證據吻合」未具名共識措辭,改為僅由 FIDELIO 次分析 HR 0.45 支持的「方向一致」敘述。
