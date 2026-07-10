# MISSING FULLTEXT — 主題候選五

主文 22 篇引用**全部 📄（本地全文，grep 可驗）**。以下為資料夾內存在但本輪未讀取內文/未引用者，以維持「全文可追溯」原則。

## 未讀取內文 → 未引用（避免自創數字）
| Paper | DOI / PMID | 處理 |
|-------|-----------|------|
| `egfr_dip_reversibility_Oh_2026`（RAAS 因果 eGFR） | **10.1111/cts.70533** / PMID 41876398 | 資料夾有檔但未讀內文;eGFR dip 預後論點改以已讀之 Ku 2024、Matsumoto 2025 支撐 |
| `r2_Holtkamp_2011`（losartan eGFR dip 預後, Kidney Int） | **10.1038/ki.2011.79** / PMID 21562470 | 同上（本輪已有本地全文 status: full_text，但正文仍以 Ku 2024/Matsumoto 2025 承擔預後論點） |
| `pooled_safety_hyperkalemia_Bakris_2020`（FIDELIO 主文, NEJM） | **10.1056/NEJMoa2025845** / PMID 33264825 | FIDELIO 安全數字改由已核實的 Agarwal 2022 與 EMA/FDA label 提供（另有本地全文 `FIDELIO-DKD_NEJMoa2025845.md`） |
| CONFIDENCE 主結果（NEJM Agarwal 2025） | **10.1056/NEJMoa2410659** / PMID 40470996 | 本地無全文;combination vs 單藥高血鉀改用已讀之 Vaduganathan 2025（NDT）Table 2 與 Agarwal 2025（GLP-1 次分析）實際數字 |
| `pooled_safety_hyperkalemia_Mentz_2025`（EJHF） | **10.1002/ejhf.3569** / PMID 39823276 | abstract-only,未使用 |
| `egfr_dip_reversibility_Oshima_2021`（Kidney Int, CREDENCE eGFR dip） | **10.1016/j.kint.2020.10.042** / PMID 33316282 | abstract-only,未使用 |

## 已補全文（本輪升級）

以下兩篇原為 abstract-only（📌），本輪經**使用者上傳之本地 PDF 經 LlamaParse 轉檔**升級為本地全文（📄，`status: full_text`，內容 grep 可驗），並已納入主文 §3.1 與參考文獻 21/22：

| Paper | 角色 | 本輪新引用之 grep 可驗數字 |
|-------|------|------|
| `pooled_safety_hyperkalemia_Neuen_2026`（INFINITY，Lancet 2026；FIDELIO+FIGARO+FIND-CKD IPD，n=14,574，含非糖尿病 CKD） | §3.1 跨試驗一致性、延伸至非糖尿病 CKD | 任一高血鉀 14·3% vs 7·6%、永久停藥 1·7% vs 0·5%、K>5·5 17·0% vs 7·9%、無高血鉀死亡 |
| `hf_renal_safety_Ostrominski_2026`（FINE-HEART pooled，2026；FIDELIO+FIGARO+FINEARTS-HF 亞群，n=14,180） | §3.1 絕對可管理性（NNT）、零高血鉀死亡 | 高血鉀住院 NNT 131、K>5.5 18% vs 8%、高血鉀相關停藥 2% vs 1%、無高血鉀死亡 |

## fetch 失敗（內容過濾）
| Paper | Reason |
|-------|--------|
| potassium binder Agarwal | workflow fetch agent 遭 content-filtering 攔下（`Output blocked by content filtering policy`）。potassium binder 論點改由已取得全文 AMBER / DIAMOND / EMCREG 支撐 |

## 稽核
citation-verifier 7 / claim-auditor 2 / cross-referencer 6；**1 條必修（ghost consensus）**已修正:§3.4 移除「與 SGLT2i 一貫降低高血鉀的 meta 證據吻合」未具名共識措辭,改為僅由 FIDELIO 次分析 HR 0.45 支持的「方向一致」敘述。
