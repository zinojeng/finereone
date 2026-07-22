---
tags: [主題, 受體藥理, 解離動力學, 類固醇型MRA對比]
created: 2026-07-22
updated: 2026-07-22
sources: [wiki/sources/2026-07-22-01-mr_receptor_dissociation_residence_time.md, wiki/sources/2026-07-22-01-01_finerenone_not_just_safer_spironolactone.md, wiki/sources/2026-07-22-01-statistical_insights_myths.md, wiki/sources/2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart.md, wiki/sources/2026-07-22-00-KDIGO_2026_Diabetes_CKD_draft.md, wiki/sources/2026-07-22-00-deep-research-report.md]
---

# 受體藥理與 nsMRA 分野

> 回答 purpose.md 關鍵問題一的前半段：finerenone 與 spironolactone 的差別，究竟有多少來自受體選擇性／解離動力學，有多少只是安全性剖面不同？

## 為什麼重要

門診最常被反問的一句話是「若效益來自 MR 阻斷，為何不用更便宜的 spironolactone？」。這一題不能只用男性女乳症回答，因為那是把「副作用譜」當成「療效等級」的答案。分子層面確實存在可量化的分野——結合口袋的立體化學、共因子招募模式、S810L 突變 MR 上的行為反轉——但這些數字全是體外藥理效價，與硬終點是不同量綱。更麻煩的是量化資料本身不對稱：finerenone 有實測解離半衰期，spironolactone 與 eplerenone 沒有，所以連「誰的 residence time 較長」都只能定性描述。真正把兩者拉開的其實是證據等級：nsMRA 有 phase 3 硬終點，類固醇型 MRA 在腎病進展上沒有。

## 素材匯總

| 素材 | 對本主題的貢獻 | 證據層級 |
|------|----------------|----------|
| [[2026-07-22-01-mr_receptor_dissociation_residence_time]] | 提供 residence time ≈ 1/koff 的框架、finerenone 三個量化錨點，並明示 spironolactone/eplerenone 的 koff 資料缺口 | 尚待驗證（in-vitro 動力學，排序資料缺） |
| [[2026-07-22-01-01_finerenone_not_just_safer_spironolactone]] | 把分子差異接到 ARTS → FIDELIO → FIGARO → FIDELITY 的硬終點證據鏈上 | 已核准（T2D+CKD） |
| [[2026-07-22-01-statistical_insights_myths]] | 拆解「500-fold 選擇性」與「至少與 spironolactone 相當」兩個量綱錯置 | 尚待驗證（頭對頭等效無證據） |
| [[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]] | 指出兩者真正的差異在 PK（代謝物）而非受體端 | 已核准（藥品標示層級 PK） |
| [[2026-07-22-00-KDIGO_2026_Diabetes_CKD_draft]] | 指引級語句：steroidal MRA 對腎病進展的效果從未在大型試驗檢驗 | 已核准（指引） |
| [[2026-07-22-00-deep-research-report]] | 誠實承認 head-to-head long-term kidney outcome data 仍不足 | 尚待驗證 |

## 核心觀點

1. **受體佔據的持久度由 koff 決定，與血中濃度是兩回事**：residence time ≈ 1/koff；血中濃度由代謝清除決定，受體佔據由分子在結合口袋卡得緊不緊決定，兩者計時完全不同（來源：[[2026-07-22-01-mr_receptor_dissociation_residence_time]]）。

2. **finerenone 的三個量化錨點**：解離半衰期 ~50 min、Kd = 1.52 ± 0.01 nM、功能性 IC50 = 58 ± 9 nM。合讀的圖像是「結合得夠緊足以有效拮抗，但解離並不慢」，並非一結合就長期黏死 📄（來源：[[2026-07-22-01-mr_receptor_dissociation_residence_time]]）。

3. **受體端親和力其實同量級**：spironolactone 功能性 IC50 為 74.0 ± 15 nM，對照 finerenone 58 ± 9 nM——效價只差約 1.3 倍。eplerenone 在另一結構研究的 transactivation 體系中 IC 為 2000 nM（同體系 spironolactone 50.0 nM、BR-4628 33.5 nM），Kolkhof 量化其對 MR 的體外親和力「約比 spironolactone 低 40-fold」📄（來源：[[2026-07-22-01-mr_receptor_dissociation_residence_time]]、[[2026-07-22-01-statistical_insights_myths]]）。

4. **spironolactone 的「黏」來自代謝物接力，不是單分子 koff**：它是 prodrug，本身血漿半衰期短，代謝出 canrenone（16.5 h）、TMS（13.8 h）、HTMS（15.0 h），穩態下以 TMS 為主（口服 100 mg/day 時 TMS 峰值相對濃度佔 50.3%）。有效受體暴露被代謝物在時間軸上拉長，不可回填成具體 off-rate 📄（來源：[[2026-07-22-01-mr_receptor_dissociation_residence_time]]、[[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]]）。

5. **結構開關是 helix 12 protrusion 與關鍵殘基接觸**：bulky 非類固醇 MRA 的 5-acetyl、C6-methyl 等基團向 H12 方向突出，使 H12 無法回到 agonist 位，形成不穩定的 receptor–ligand 複合體、無法招募共因子。mutagenesis 指出 spironolactone/progesterone 無法與 Asn770 建立強接觸是其被動拮抗特徵之源；Amazit 以突變體鎖定 Ser-810 與 Ala-773 為 finerenone 高選擇性的關鍵殘基 📄（來源：[[2026-07-22-01-mr_receptor_dissociation_residence_time]]）。

6. **共因子行為出現定性反轉**：在 [[SCNN1A]] 調控序列的 ChIP 分析中，finerenone 抑制 MR、SRC-1 與 RNA polymerase II 招募，並顯著降低基礎狀態下 MR 與 SRC-1 的結合，呈現 [[inverse agonist]] 特性；spironolactone 在同一序列上表現為 partial agonist 📄（來源：[[2026-07-22-01-01_finerenone_not_just_safer_spironolactone]]、[[2026-07-22-01-mr_receptor_dissociation_residence_time]]）。

7. **[[S810L 突變 MR]] 是安全藥理學的分水嶺**：S810L 是造成早發、懷孕期惡化之高血壓的活化型突變，spironolactone 在其上轉為強效致效劑因而屬禁忌（EC50 = 25 ± 2 × 10⁻¹¹ M）；finerenone 維持嚴格拮抗（IC50 = 16.1 ± 3.1 × 10⁻⁶ M）📄（來源：[[2026-07-22-01-01_finerenone_not_just_safer_spironolactone]]、[[2026-07-22-01-mr_receptor_dissociation_residence_time]]）。

8. **「500-fold 選擇性」是效價比，不是效益倍數**：該選擇性是對照 65 個受體與離子通道（含 L-type Ca²⁺ channel）測出，正確的臨床翻譯是副作用譜更乾淨與分子行為可預測；「有多少心腎保護」只能由 RCT 的 HR/NNT 回答 📄（來源：[[2026-07-22-01-statistical_insights_myths]]）。

9. **真正拉開分野的是證據等級，不是分子**：類固醇型 MRA 仍是 HFrEF、原發性醛固酮症、頑固型高血壓的標準治療，但其對腎病進展（eGFR 下降或腎衰竭）的效果未在大型試驗檢驗過，且高血鉀風險增 2–3 倍、AKI 增 2 倍；KDIGO 2026 草案的 Practice Point 4.4.7 明令兩者不得併用，且 nsMRA 不能取代 steroidal MRA 於 HFrEF（<40%）與醛固酮增多症的適應症（來源：[[2026-07-22-00-KDIGO_2026_Diabetes_CKD_draft]]）。

## 尚有爭議或未解之處

1. **只有 finerenone 有實測解離半衰期**：spironolactone 與 eplerenone 各自的解離半衰期／koff／residence time，本地與已檢索學術來源皆未提供定量值，也不存在三者並列的 kon/koff 表。任何「residence time 排序」只能作定性描述（來源：[[2026-07-22-01-mr_receptor_dissociation_residence_time]]）。**尚待驗證**

2. **「至少與 spironolactone 相當」是 absence of evidence**：ARTS 是 phase II、主終點為血清鉀變化，生物標記全屬 exploratory；原文明寫 part B 對 BNP、NT-proBNP、UACR 未見顯著整體療效（P > 0.05），因此未計算個別組間 P 值、僅作描述性分析。其樣本量是為偵測 K⁺ 差 0.26 mmol/L 而算（來源：[[2026-07-22-01-statistical_insights_myths]]）。**尚待驗證**

3. **唯一的頭對頭是 90 天生物標記試驗**：ARTS-HF（finerenone vs eplerenone）以「NT-proBNP 下降 >30% 比例」為主終點，兩組達標比例相近（eplerenone 37.2% vs finerenone 各劑量 30.9–38.8%，P = 0.42–0.88）；探索性臨床複合終點 HR 0.56（0.35–0.90，nominal P = 0.02）但未為此設計檢力。「finerenone 硬終點優於類固醇型 MRA」目前無證據（來源：[[2026-07-22-01-01_finerenone_not_just_safer_spironolactone]]）。**尚待驗證**

4. **分子差異與臨床差異之間隔著一次未經檢驗的外推**：所有 finerenone 硬終點試驗的對照組皆為安慰劑，長期腎臟硬終點的頭對頭比較不存在；把 in-vitro 的共因子調節差異直接讀成臨床優勢，是跨量綱的推論（來源：[[2026-07-22-01-statistical_insights_myths]]、[[2026-07-22-00-deep-research-report]]）。<!-- confidence: INFERRED -->

5. **11β-HSD2 的組織分布意味 MR 的主要配體可能不是醛固酮**：滅活皮質醇的 11β-HSD2 存在於遠端腎元上皮，但在心肌細胞、podocyte 與巨噬細胞中不存在，因此在這些細胞中豐度更高的皮質醇可能才是 MR 的主要活化配體（來源：[[2026-07-22-01-01_finerenone_not_just_safer_spironolactone]]）。這對「阻斷受體 vs 降低醛固酮」的策略選擇有直接含義。<!-- confidence: INFERRED -->

## 關鍵實體

- [[礦皮質素受體]] — 本主題的共同標的；其在上皮與非上皮組織的配體差異決定了兩類 MRA 的分野邊界
- [[受體滯留時間]] — 把「結合多緊」與「血中還有多少藥」分開的核心概念，也是資料缺口最大的一格
- [[Finerenone]] — 唯一有實測 koff、且唯一有 phase 3 硬終點的 nsMRA
- [[Spironolactone]] — 受體端親和力與 finerenone 同量級，差別在代謝物 PK 與選擇性
- [[Eplerenone]] — 定位是選擇性而非親和力；體外親和力低但臨床效價落差說明結合實驗不能授權劑量
- [[Esaxerenone]] — 另一個 nsMRA，其「至少 1000-fold 選擇性」與 finerenone 的 500-fold 同屬效價比語言
- [[inverse agonist]] — finerenone 在基礎狀態即壓低 MR–SRC-1 結合，與 spironolactone 的 partial agonist 行為相反
- [[S810L 突變 MR]] — 讓兩藥行為完全反轉的天然實驗，是安全藥理學上最乾淨的分野證據
- [[SCNN1A]] — ENaC α 次單元基因，共因子招募差異的觀測場域
- [[ARTS-DN]] — 從受體藥理走向臨床劑量選擇的橋樑試驗

## 相關頁面

- [[PK-PD 解耦與停藥可逆性]]
- [[BP-independent 心腎保護]]
- [[合成端 vs 受體端：ASI 與原發性醛固酮症]]
