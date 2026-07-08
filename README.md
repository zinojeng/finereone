# Finerenone 心腎保護：進階演講題庫（七大主題深度文獻回顧）

給**內分泌科醫師**的 finerenone / 非類固醇型礦皮質素受體拮抗劑（nsMRA）進階演講素材。聽眾已熟悉 FIDELIO-DKD / FIGARO-DKD / FIND-CKD 等試驗名稱與 finerenone 的基本心腎益處；本題庫刻意壓縮背景（約 20–40%），把重心（約 70%）放在更深的次分析、機制與 editorial 級討論。

每個主題各自成一個資料夾，含：主文 `.md`、`原始PDF/`（本地全文語料，供 grep 稽核）、`MISSING_FULLTEXT.md`（未取得全文/abstract-only/污染 PDF 紀錄）、`撰寫方法論.md`（當次管線紀錄）。

## 七大主題

| # | 主題 | 核心切入 | 主文 |
|---|------|----------|------|
| 1 | **Finerenone 不只是比較安全的 spironolactone** | receptor pharmacology、非類固醇選擇性、BP-independent 心腎保護；分子→生物標記→臨床三層 | [`01_...`](01_finerenone_not_just_safer_spironolactone/) |
| 2 | **從白蛋白尿到硬終點** | UACR 作為 companion biomarker vs mechanism-linked surrogate；eGFR slope 資格化方法學 | [`02_...`](02_albuminuria_to_hard_endpoints/) |
| 3 | **第四支柱還是提早聯用** | RASi+SGLT2i 之後,finerenone 序列加藥 vs 同步起始;CONFIDENCE 三臂 | [`03_...`](03_fourth_pillar_or_early_combination/) |
| 4 | **誰得到最大效益** | subgroup / effect-modification;who-to-treat-first(絕對事件率)> who-benefits-most | [`04_...`](04_who_gets_greatest_benefit/) |
| 5 | **高血鉀與 eGFR dip 的安全工程學** | protocolized monitoring;場景別高血鉀、eGFR dip 可逆性、CYP3A4、K binder、門診 workflow | [`05_...`](05_hyperkalemia_egfr_dip_safety_engineering/) |
| 6 | **超越 T2D 的心腎版圖** | FINE-ONE(T1D)、FIND-CKD(非DM)+glomerular 亞群、FINE-HEART pooled;CKM platform | [`06_...`](06_beyond_t2d_cardiorenal_landscape/) |
| 7 | **Aldosterone synthase inhibitor(ASI）vs finerenone** | 合成端 vs 受體端機轉;finerenone 不過 BBB → stroke 中性(FIGARO HR 0.97);ASI 結局是否一致（待驗證假說） | [`07_...`](07_aldosterone_synthase_inhibitor_vs_finerenone/) |

> [`deep-research-report.md`](deep-research-report.md) 為產生前六個主題的母體研究報告（含各主題完整 面向 brief、試驗/法規里程碑、優先文獻地圖）。主題七為後續加開的機轉對比題（ASI：baxdrostat / lorundrostat / vicadrostat）。

## 涵蓋的核心試驗與分析
ARTS / ARTS-DN / ARTS-HF · FIDELIO-DKD · FIGARO-DKD · FIDELITY(個體層級 pooled) · FINEARTS-HF(HFpEF/HFmrEF) · CONFIDENCE(finerenone+empagliflozin 三臂) · FINE-ONE(T1D) · FIND-CKD(非糖尿病 CKD)+glomerular 亞群 · FINE-HEART pooled(18,991) · INFINITY / 2026 Lancet DM+非DM pooled · ASI：BrigHTN / BaxHTN / Launch-HTN / Advance-HTN / EASi-KIDNEY。

## 撰寫方法與可信度
全部主題以 `medical-literature-review` skill 的多 agent 管線產生：**多源搜尋（paper-search-mcp 21 來源）→ OA-first 全文下載 → 第二輪深挖共引 seminal papers → 撰稿 → citation/claim/cross-ref 三方敵對稽核 → 修正**。

硬規則：**LLM 只做組織與改寫;所有作者/年份/DOI/數字/樣本數/HR 必須能 grep 回本地全文**。
- 📄 = 本地全文驗證　📌 = 僅 abstract（不對其未載內容作具體數字斷言）
- 每個 abstract-only、付費牆、或污染 PDF 事件都在各主題 `MISSING_FULLTEXT.md` 誠實揭露
- 每篇主文文末以「已核准 / 可外推 / 尚待驗證（surrogate-based / hypothesis）」層級標示證據性質

---
*資料日期基準：2026-07-08。FDA 對 finerenone T1D-CKD 適應症當時僅「受理 Priority Review」，尚非核准。ASI 目前多為 BP/surrogate 證據，EASi-KIDNEY 為首個 ASI hard-outcome phase 3（進行中）。*
