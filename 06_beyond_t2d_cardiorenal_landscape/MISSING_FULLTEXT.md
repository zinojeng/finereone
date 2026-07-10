# MISSING FULLTEXT — 主題候選六

本主題多為 2026 年新發表、付費牆/無 OA 論文,故 📌（abstract-only）比例偏高;所有 abstract-only 數字均取自已比對 title/DOI/PMID 的結構化 abstract,未對未載內容作斷言。

## 僅 abstract（📌）— 付費牆/無 OA,只用結構式 abstract 數字
| Paper | DOI / PMID | 內容 |
|-------|-----------|------|
| （本輪 T1D/FINE-ONE 三篇已全部升級為本地全文,詳見下方「## 已補全文（本輪升級,round 2）」小節） | — | — |

## 已補全文（本輪升級,round 2）
以下三篇 FINE-ONE 相關論文由**使用者上傳之本地 PDF,經 LlamaParse 轉為 Markdown** 落地為本地全文（status: full_text,📄 可 grep 稽核）,本輪自上方「僅 abstract（📌）」表移除;正文對應句之 📌 已逐一 grep 驗證數字後改為 📄。

| Paper（本地 MD 檔） | DOI / PMID | 正文已升級之關鍵數字（均 grep 命中） |
|-------|-----------|------|
| fine_one_t1d_Heerspink_2026.md（FINE-ONE NEJM 本體） | **10.1056/NEJMoa2512854** / PMID 41780000 | n=242、UACR −34%（GMR 0.66,0.60–0.73）/placebo −12%（0.88,0.79–0.98）/placebo-corrected −25%（GMR 0.75,0.65–0.87,P<0.001）、高血鉀 10.1%(12) vs 3.3%(4)、停藥 1.7%(2)、eGFR −5.6 vs −2.7（差 −2.9,−5.1 至 −0.7）;新補 responder ≥30%/≥50%:54.3%/28.4% vs 32.7%/21.8% |
| fine_one_t1d_Beernink_2026.md（HbA1c/病程次組, Diabetes Care） | **10.2337/dc26-0882** / PMID 42258447 | HbA1c 三分位 Pint=0.41、病程三分位 Pint=0.70、6 月 HbA1c 組間差 +0.04%（P=0.74）、placebo-corrected −25% |
| fine_one_t1d_Heerspink_2023.md（FINE-ONE 設計, Diabetes Res Clin Pract） | **10.1016/j.diabres.2023.110908** / PMID 37805000 | primary=6 月 UACR 相對變化、UACR 作 bridging biomarker、經 regulatory authority feedback 同意作 T1D 註冊橋接、NCT05901831 |

## 已補全文（前輪升級）
以下論文由**使用者上傳之本地 PDF,經 LlamaParse 轉為 Markdown** 落地為本地全文（status: full_text,📄 可 grep 稽核）。原先列於「僅 abstract（📌）」者已自上表移除,正文對應句之 📌 已逐一 grep 驗證數字後改為 📄。

| Paper（本地 MD 檔） | 正文已升級之關鍵數字（均 grep 命中） |
|-------|------|
| find_ckd_nondiab_Heerspink_2026.md（FIND-CKD NEJM 本體） | n=1584（793/791）、eGFR slope 差 0.7（0.3–1.1）、cardiorenal HR 0.77（0.60–0.99）、腎複合 0.78、CV 複合 0.60（0.27–1.33）、高血鉀 17.0% vs 13.3% |
| find_ckd_nondiab_Neuen_2026.md（INFINITY / Lancet pooled） | n=14,574、腎複合 HR 0.76（0.68–0.86）、kidney failure 0.85（0.74–0.99）、CV 複合 0.80（0.70–0.91）、HHF 0.78（0.66–0.92）、CV 死亡 0.82（0.67–0.999）、全因死亡 0.88（0.79–0.99）(檔內以中點「·」為小數點) |
| glomerular_subgroup_Neuen_2026.md（Glomerular JAMA 亞群） | n=903（57.0%）、IgAN 416（46.1%）/FSGS 215（23.8%）/MN 90（10.0%）、slope 差 0.73（0.22–1.24）、白蛋白尿 −42%（35–48%）、腎複合 7.42 vs 9.60/100PY HR 0.74（0.57–0.97）；新補：腎切片確診 712/903（78.8%）敏感度分析 HR 0.74（0.55–0.99） |
| finearts_hfpef_ckm_Ostrominski_2026.md（FINE-HEART CKD 子集 JASN） | n=14,180、CV 死亡/HHF HR 0.83（0.75–0.93,P=0.001）、腎複合益處隨 UACR 升高（Pint=0.04）、非糖尿病敏感度 HbA1c Pint=0.59 |
| hf_finearts_Solomon_2024.md、hf_finearts_Vaduganathan_2024.md、finearts_baseline_ejhf_Solomon_2024.md、finearts_hfpef_ckm_Vaduganathan_2024.md | FINEARTS-HF 本體/基線相關全文,本輪已落地但正文既有分析未引用其新數字,未作擴張 |
| arts_hf_Filippatos_2016.md（ARTS-HF,新增檔） | 先前遭 content-filter 阻擋、無本地檔;本輪新增本地全文。正文目前未引用,列此備查 |

## ⚠️ 上傳檔名與內容不符 → 已分檔處理
- 使用者上傳的 `Foà 猝死 2026.pdf` 檔名雖為「猝死」,但 PDF 實際內容為 **Foà 等「Finerenone-Related Risk of Hypotension in HFmrEF/HFpEF」(JACC Heart Fail. 2026;14(4):102779)**——SBP ≤100 mmHg / 低血壓分析,**並非**正文所引之「猝死（sudden death）FINE-HEART 分析」。
- **處理**:
  1. `finearts_hfpef_ckm_Foa_2026.md`（猝死）**維持原 abstract-only 📌 stub 不變**;正文猝死數字(418、2.2%、HR 0.81、95% CI 0.67–0.98、P=0.034)及 Ameri editorial 於低血壓全文 grep 不到,故正文第 82、169 行與 References #16 之 📌 **維持不變**,待取得正確之 Foà 猝死全文再升級。
  2. 低血壓全文另存為新檔 **`finearts_hfpef_ckm_Foa_hypotension_2026.md`（status: full_text）**,front-matter 以其真實身分（DOI 10.1016/j.jchf.2025.102779）標示;正文目前未引用,列此備查。

## brief 指定但本地無全文 → 未引述其內容（依硬規則不自創引用）
- **NEJM 的 T1D editorial**《Finerenone for Diabetic Kidney Disease in Type 1 Diabetes》
- **Lancet 的**《Finerenone: kidney protection beyond type 2 diabetes》editorial

本地目錄無對應 MD 檔,已於 Discussion 明確標註「未取得本地全文」。本地唯一可稽核之伴隨評論為 Foà 檔內記載的 **Ameri 2026 JACC editorial comment**,已列入 References。

## FDA 狀態精確標示
截至 2026-07-08,FDA 對 T1D-CKD 僅「受理 Priority Review」,尚非核准——已於正文精確標示。

## 誠實揭露的反向訊號
FINEARTS-HF 場景中 Mc Causland 的腎複合 HR 1.33（反向）已納入 discussion,作為 HF/CKD pooling 詮釋邊界的保留。

## 稽核
citation-verifier 5 / claim-auditor 1 / cross-referencer 9;**2 條必修**（References #13 Docherty 2025 Circulation、#14 Mc Causland 2025 JACC 補正卷期頁與 DOI,經本地 front-matter 佐證）已修正。
