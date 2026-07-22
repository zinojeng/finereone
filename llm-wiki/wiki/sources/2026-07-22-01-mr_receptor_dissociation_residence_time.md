---
tags: [素材摘要, 受體藥理與解離動力學, 結構生物學, 藥理對比]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/01-mr_receptor_dissociation_residence_time.md
images: 0
image_paths: []
---

# MR 受體的解離動力學與駐留時間

> 受體佔據的持久度由解離速率常數 koff 決定（residence time ≈ 1/koff），與血中濃度是兩回事；finerenone 有唯一的實測錨點（解離半衰期 ~50 min），spironolactone/eplerenone 的 koff 定量值本地全無，不可杜撰。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/01-mr_receptor_dissociation_residence_time.md
- **消化日期**：2026-07-22

## 核心觀點

1. **residence time 的藥理框架**：受體被佔據的持久度取決於藥物從受體鬆手的速度（off-rate, koff），而非血中游離濃度；residence time ≈ 1/koff。血中濃度由代謝清除（CYP、腎排）決定，受體佔據由分子在結合口袋裡卡得緊不緊決定——兩者計時完全不同。此為藥理框架（🟡 可詮釋），本身不帶數字。

2. **finerenone 的三個量化錨點**：解離半衰期 ~50 min、Kd = 1.52 ± 0.01 nM（與 in vitro 轉譯之全長 MR 結合）、功能性 IC50 = 58 ± 9 nM，皆出自 📄[molecular_Amazit_2015.md]。三者合讀的圖像是：結合得夠緊（奈莫耳級 Kd）足以有效拮抗，但解離並不慢（~50 min），並非「一結合就長期黏死」。**🟡 in-vitro kinetic**。

3. **結構型態與動力學的對應**：finerenone 屬 bulky-passive 拮抗；Fagart 把 passive 拮抗劑歸為「會快速從受體解離的小分子」，並以 BR-4628 從 MR 的快速解離（原檔關鍵詞 `quickdissociation`）佐證 MR·BR-4628 複合體無法形成穩定構型 📄[r2_Fagart_2010.md]。本檔核心洞見是把兩者放在同一因果線：複合體不穩定（塞不緊）→ koff 較大 → residence time 較短。**🟡 機轉外推**。

4. **spironolactone 的受體端親和力與 finerenone 同量級**：功能性 IC50 74.0 ± 15 nM（對照 finerenone 58 ± 9 nM）📄[molecular_Amazit_2015.md]；另一結構研究的 transactivation 體系中 spironolactone IC 為 50.0 nM（同體系 BR-4628 33.5 nM）📄[r2_Fagart_2010.md]。也就是「結合有多緊」兩者相近。

5. **spironolactone 的「黏」來自代謝物接力而非單分子 koff**：它是 prodrug，本身血漿半衰期短，卻代謝出三個長效活性代謝物——canrenone（16.5 h）、TMS（13.8 h）、HTMS（15.0 h），穩態下以 TMS 為主 📄[molecular_Kolkhof_2017.md]。分子層面的意義是「有效受體暴露」被代謝物在時間軸上拉長，而非某一顆分子的 residence time 變長。**🟡 推論，不可回填成具體 off-rate**。

6. **型態反轉與 coregulator 行為**：S810L 突變 MR 上 spironolactone 轉為 agonist（EC50 = 25 ± 2 × 10⁻¹¹ M），finerenone 維持嚴格拮抗（IC50 = 16.1 ± 3.1 × 10⁻⁶ M）📄[molecular_Amazit_2015.md]。spironolactone 與 BR-4628 一樣不促使 MR 招募 NCoR，且抑制 NCoR 與 MR-aldosterone 複合體結合 📄[r2_Fagart_2010.md]；在 SCNN1A 上 spironolactone 表現為 partial agonist，與 finerenone 的 inverse agonist 相反 📄[molecular_Kolkhof_2017.md]。

7. **eplerenone 的定位是選擇性而非親和力**：transactivation IC 為 2000 nM（同體系 spironolactone 50.0 nM、BR-4628 33.5 nM）📄[r2_Fagart_2010.md]；Kolkhof 量化其對 MR 的 in vitro 親和力「約比 spironolactone 低 40-fold」📄[molecular_Kolkhof_2017.md]。其環氧修飾降低對 AR/PR 的親和 → 選擇性優於 spironolactone；in vivo 以較高游離比例（血漿蛋白結合約 50%，spironolactone 94%）部分補償低親和力。finerenone 對 MR 的選擇性再進一階——至少 500-fold 相對於 eplerenone，且效價至少等同 spironolactone 📄[molecular_Kolkhof_2017.md]。

8. **結構開關：helix 12 protrusion 與 Asn770**：bulky 非類固醇 MRA 的 5-acetyl、C6-methyl 等基團向 H12 螺旋方向突出（`protrude toward the H12 helix`），使 H12 無法回到 agonist 位；Kolkhof 綜述總結 bulky MRA「probably cause a protrusion of helix 12 … and as a consequence, an unstable receptor–ligand complex, which is unable to recruit coregulators」📄[molecular_Kolkhof_2017.md]。BR-4628 docking 到 agonist conformation 卻因與 D-ring 錨定區（Thr945）無接觸而無法形成穩定複合體 📄[r2_Fagart_2010.md]。mutagenesis 指出 spironolactone/progesterone 無法與 Asn770 建立強接觸是其被動拮抗特徵之源，BR-4628 則強烈接觸 Asn770；Amazit 以突變體鎖定 Ser-810 與 Ala-773 為 finerenone 高選擇性的關鍵殘基 📄[molecular_Amazit_2015.md]。

9. **核轉位與 cofactor 抑制的功能後果**：aldosterone 單獨誘導最大 translocation index 3.11 ± 0.02；拮抗劑單獨（1 h）僅輕度上升（spironolactone 1.84 ± 0.01、finerenone 1.76 ± 0.01），且 finerenone 比 spironolactone 更有效延遲 aldosterone 誘導的 MR 核輸入 📄[molecular_Amazit_2015.md]。

10. **明示缺口（🔴 尚待驗證）**：只有 finerenone 有實測解離半衰期；spironolactone 與 eplerenone 各自的解離半衰期／koff／residence time，本地與已檢索學術來源（含 Consensus／PubMed 檢索）未提供定量值，也不存在三者並列的 kon/koff 表。任何「residence time 排序」只能作定性描述，避免製造排序幻覺。

## 關鍵概念

- [[受體滯留時間]]
- [[受體滯留時間]]
- [[礦皮質素受體]]
- [[礦皮質素受體]]
- [[礦皮質素受體]]
- [[S810L 突變 MR]]
- [[inverse agonist]]
- [[Finerenone]]
- [[Spironolactone]]
- [[Eplerenone]]

## 與其他素材的關聯

- 與 `01-pk_pd_hysteresis_offrate_hold_restart.md` 是原文明示的**姊妹檔**關係：本檔專注受體結合的微觀物理，姊妹檔談三個時鐘（PK 清除／off-rate／PD 重建）的臨床耦合與 hold-restart，兩檔刻意不重複。<!-- confidence: EXTRACTED -->
- 與 `01-01_finerenone_not_just_safer_spironolactone.md` 是**深化**關係：主文表 1 列出的「親和力、輔因子招募、S810L 行為、組織分布」在本檔被展開為結構與動力學的因果鏈。<!-- confidence: EXTRACTED -->
- 與 `01-statistical_insights_myths.md` 的迷思一（500-fold 選擇性不是效益倍數）直接互補：本檔提供效價只差約 1.3 倍（58 vs 74 nM）的原始數字。<!-- confidence: INFERRED -->
- 原文對 Fagart 檔的英文逐字引句因 PDF 轉檔字元黏連而多採中文概念改寫，僅保留可 grep 命中的關鍵詞——引用該檔的 verbatim 句子時需注意此限制。<!-- confidence: AMBIGUOUS -->

## 原文精彩摘錄

> 把 MR 想成一把鎖，拮抗劑是插進去的鑰匙。PK 半衰期問的是「櫃檯（血液）還有幾把備用鑰匙」；residence time 問的是「已經插進鎖孔的這把鑰匙，卡得多緊、多久會自己滑出來」。兩個問題的答案可以完全不同。

> MR 的 H12 像一道要「喀」一聲扣上才會啟動下游的門閂。類固醇型（spiro/eple）體積合身、不去頂那道門閂，屬「被動不啟動」；bulky 非類固醇（fine/BR-4628）則像塞了一個過大的楔子，把門閂頂歪——門關不上（無法招募 coregulator），而且楔子本身塞不穩、容易滑出（解離快）。

> spironolactone 的「受體端更持久」實為代謝物接力延長有效暴露而非單分子 koff 變小；eplerenone 由低親和力框架推測 koff 偏大。不杜撰 spiro/eplerenone 的具體 off-rate 數字。

## 相關頁面
