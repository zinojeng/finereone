# MISSING FULLTEXT — 主題候選四

## 僅 abstract（📌）— 只用其公開摘要數字,不作具體數字擴張斷言
| Paper | DOI / PMID | 內容 | Reason |
|-------|-----------|------|--------|
| `baseline_goals_absolute_Zuin_2026`（fragility 分析） | **10.1093/ejhf/xuag150** / PMID 42087276 | fragility index 細節未取得，故未斷言 | OUP 付費牆 |
| `baseline_goals_absolute_Zhao_2026`（胰島素阻抗, n=45 單中心） | **10.1111/jdi.70368** / PMID 42332386 | 僅列為機轉假說；使用者上傳之 PDF 實為另一篇 islet-pathology 論文，非該 finerenone 胰島素阻抗研究，故 📌 保持不變 | 小樣本真實世界 / 上傳 PDF 不符 |

## 已補全文（本輪升級，round 2）
來源：使用者上傳本地 PDF 經 LlamaParse 轉檔（status: full_text，內文可 grep）。原標 📌 之數字/敘述均已 grep 回本地全文 MD 命中，主文與 References 相應標記改為 📄。
| Paper | DOI / PMID | 已 grep 命中之關鍵內容 |
|-------|-----------|------|
| `stage4_ckd_Bakris_2023`（Kidney Int, FIDELITY 腎臟探索性分析） | **10.1016/j.kint.2022.08.040** / PMID 36367466 | ≥57% 腎臟複合 HR 0.77(0.67–0.88)、3 年 ARR 1.7%(0.7–2.6)、P_interaction 0.62/0.67、ESKD HR 0.80(0.64–0.99)、血鉀停藥 eGFR<60 vs ≥60 = 2.4% vs 0.6% |
| `asian_subgroup_Li_2024`（Cardiorenal Med review） | **10.1159/000538347** / PMID 38537621 | "Due to the limited data for subgroups, it is prudent to approach the conclusion with caution"（原文逐字，主文為改寫） |
| `r2_Agarwal_2025`（CONFIDENCE NEJM） | **10.1056/NEJMoa2410659** / PMID 40470996 | 併用比單用 finerenone 多降 UACR 29%、比單用 empagliflozin 多降 32%、併用組 180 天 UACR 降 52%、AE uncommon |
| `r2_Bakris_2015`（ARTS-DN） | **10.1001/jama.2015.10081** / PMID 26325557 | 僅 References 引用，無內文數字斷言；全文已落地，標記改 📄 |
| `r2_Solomon_2024`（FINEARTS-HF, NEJM） | **10.1056/NEJMoa2407107** / PMID 39225278 | 僅 References 引用，無內文數字斷言；全文已落地，標記改 📄 |

## 未納入正文的本地檔（方法學重複，已由同類全文覆蓋）
subgroup_methodology 的 Sun_2012 / Schandelmaier_2019 / Kasenda_2014 / Liu_2019 / Hayward_2006 / Sun_2014 / Rothwell_2005 多數未直接引用；核心方法學已由全文 Sun_2010、Yusuf_1991、Assmann_2000、Wallach_2017、ICEMAN(Schandelmaier_2020)、Kent_2016/2018、Matsushita_2010 充分支撐。

## 稽核
citation-verifier 4 / claim-auditor 4 / cross-referencer 3；**1 條必修**（References #10 Sato 2024 FOUNTAIN 缺 DOI → 補正 J Clin Med. 2024;13(17):5107, doi:10.3390/jcm13175107, PMID 39274317；經 CrossRef 佐證，內文數字 N=1029 等全部正確）已修正。
