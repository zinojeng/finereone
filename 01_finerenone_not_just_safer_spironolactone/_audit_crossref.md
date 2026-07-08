# Cross-reference 稽核報告
稽核對象:`01_finerenone_not_just_safer_spironolactone.md`
稽核員:cross-referencer(Phase B)
稽核方法:逐條比對正文 📄/📌[檔名] 標註 與 `原始PDF/` 本地全文,並比對 References 1–22 號清單與正文引用檔名之對應關係。

## 稽核範圍與方法說明
本文不使用傳統 `[N]` 數字內文引用,而是以 `📄[檔名]` / `📌[檔名]` 標註於句末,References 區塊(1–22 號)再將檔名對應到完整 Vancouver 格式書目。因此本次「序號 range check」改以下列方式執行:
1. 抽取正文所有 `📄/📌[檔名]` 出現次數與種類(共 23 個相異檔名)。
2. 比對 References 1–22 號清單的檔名(共 22 個)。
3. 對高頻率、高影響力的數字性論斷(HR、95% CI、P 值、IC50、Kd 等)逐一 grep 本地全文核對。
4. 搜尋 ghost consensus 慣用語(許多研究/多數證據/普遍認為/通常等)。
5. 檢查 synthesis overreach(A 證明 X 故 Y 型推論)。
6. 檢查時序邏輯(2026 年文獻是否引用了更晚的研究)。

---

## 發現一:Dead-link — 正文引用檔名未列入 References 清單

**嚴重度:必修**

**原文位置**(第 154 行):
> 「FIDELIO/FIGARO 的方案為初始 10 mg(eGFR 25–<60)或 20 mg(eGFR ≥60),目標 20 mg/day,當 K⁺ >5.5 mmol/L 時暫停、降至 ≤5.0 再恢復📄[_prior_fidelio_figaro_extract.md]。」

**問題類型**:dead-link(reference-list gap)

**問題說明**:正文使用 `📄[_prior_fidelio_figaro_extract.md]` 作為來源標註,但 References 區塊(第 176–220 行,編號 1–22)中**沒有任何一條對應此檔名**。全文所有 📄/📌 標註共出現 23 個相異檔名,但 References 只有 22 條,差額正是這個檔案。核對 `原始PDF/_prior_fidelio_figaro_extract.md` 內容,確認其為 FIDELIO-DKD(ref #6)與 FIGARO-DKD(ref #7)兩篇試驗的方法學摘錄整理稿(非獨立發表之論文),其中確實記載「Initial dose 10 mg/day if eGFR 25 to <60, 20 mg/day if eGFR >=60; target 20 mg/day. Drug withheld if K+ >5.5 mmol/L, restarted when <=5.0」,與正文論斷內容相符,不是憑空捏造的數字;但作為一個「有 📄 標記卻無編號書目條目」的檔案,違反了本文自訂的稽核公約(「每一項事實性論斷句末以 [本地MD檔名] 標註可回溯來源」隱含應可回溯至 References)。若讀者依 Vancouver 格式尋找此來源,將找不到對應條目,屬於格式層次的 dead-link。

**建議修法**:
- 選項 A(建議):將該句尾的 `📄[_prior_fidelio_figaro_extract.md]` 改為已存在於 References 的 `📄[FIDELIO-DKD_NEJMoa2025845.md] / 📄[FIGARO-DKD_NEJMoa2110956.md]`(即 ref #6 / #7),因為劑量方案本就出自這兩篇試驗的 Methods,不需要額外的摘錄檔案作為獨立來源。
- 選項 B:若要保留 `_prior_fidelio_figaro_extract.md` 作為獨立可追溯節點,應在 References 補上第 23 條「FIDELIO-DKD/FIGARO-DKD 方法學摘錄(內部整理稿,衍生自 ref #6、#7)」並說明其性質,避免造成「有標註、無編號」的落差。

---

## 發現二:References 第 5 條缺少 DOI(格式一致性)

**嚴重度:待議**

**原文位置**(第 186 行):
> 「5. Pitt B, Kober L, Ponikowski P, Gheorghiade M, Filippatos G, Krum H, et al. Safety and tolerability of the novel non-steroidal mineralocorticoid receptor antagonist BAY 94-8862 in patients with chronic heart failure and mild or moderate chronic kidney disease: a randomized, double-blind trial. Eur Heart J. 2013;34(31):2453-2463. 📄[arts_program_Pitt_2013.md]」

**問題類型**:格式不一致(非事實錯誤)

**問題說明**:文件標題明示「References(Vancouver 風格,**含 DOI**)」,References 1–22 中僅第 5 條(ARTS,Pitt 2013)未附 DOI,其餘 21 條皆有。核對本地檔案 `arts_program_Pitt_2013.md` frontmatter,確實存在 `doi: "10.1093/eurheartj/eht187"`,可直接補上,不影響事實正確性,純屬遺漏。

**建議修法**:在第 5 條句尾補上 `doi:10.1093/eurheartj/eht187`,與其餘條目格式一致。

---

## 發現三:Amazit 2015 本地全文自帶「來源可信度但需人工核對」但正文未承接此警示

**嚴重度:待議**

**原文位置**:第 3.3、3.4 節與表 1 中多處引用 `📄[molecular_Amazit_2015.md]` 的 IC50、Kd、核轉位指數、S810L IC50 等數字(第 46–54、91 行)。

**問題類型**:provenance risk(非 misattribution——數字本身經逐一 grep 核對皆準確)

**問題說明**:本地檔案 `molecular_Amazit_2015.md` 開頭明確註記:「The full-text XML was not openly deposited...Introduction / Results / Methods / Discussion / figure-legend content...was extracted from the PMC full-text HTML page via WebFetch; quantitative values...are copied from that page. **Cross-check numbers against the publisher PDF before quoting in a manuscript.**」也就是說,此檔案本身承認其數字擷取自次級 HTML 頁面而非正式 PDF,存在潛在轉錄誤差風險。逐一核對後(IC50 58±9 vs 74.0±15 nM、Kd 1.52±0.01 nM、半衰期 ~50 min、轉位指數 3.11±0.02、S810L IC50 16.1±3.1×10⁻⁶ M),這些數字在正文中被完整且正確地轉錄,且與 Kolkhof 2017(獨立文獻)在質性結論上互相印證(inverse agonist、S810L 嚴格拮抗、延遲核轉位),風險應屬可控。但正文並未在稽核說明或限制段落中提及此項來源本身帶有的「未經出版社 PDF 覆核」警語,對於一篇強調可追溯性的文件而言,建議至少在第 6 節「誠實承認的限制」中補充一句提示。

**建議修法**:在第 6 節「誠實承認的限制」段落追加一句,例如:「此外,Amazit 2015 之量化數值(IC50、Kd 等)係由 PMC 全文 HTML 頁面擷取而非出版社 PDF 原文,雖與 Kolkhof 2017 之質性結論互相印證,仍建議未來版本以出版社 PDF 覆核精確數值。」

---

## 已核對且判定「通過」的重點論斷(供 arbitrator 參考,未列入問題清單)

以下為高權重數字性論斷,已逐一 grep 本地全文核對無誤(數值、方向、統計顯著性、單位皆與來源一致),未發現 misattribution 或 overreach:

- FIDELIO-DKD 主終點 HR 0.82(0.73–0.93,P=0.001)、3 年 NNT 29、次要 CV 複合終點 HR 0.86(0.75–0.99,P=0.03)——與 `FIDELIO-DKD_NEJMoa2025845.md` 完全一致。
- FIGARO-DKD 主終點 HR 0.87(0.76–0.98,P=0.03)、HHF 驅動 HR 0.71(0.56–0.90)——與 `FIGARO-DKD_NEJMoa2110956.md` 完全一致。
- FIDELITY N=13,026、CV HR 0.86(0.78–0.95,P=0.0018)、腎臟 HR 0.77(0.67–0.88,P=0.0002)、ESKD HR 0.80(0.64–0.99)、RAS 99.8%、SGLT2i 6.7%、UACR ratio 0.68(0.66–0.70)、SBP −3.2 vs +0.5 mmHg——與 `biomarker_Agarwal_2022.md` 完全一致。
- ARTS 血清鉀 0.04–0.30 vs 0.45 mmol/L(P<0.0001–0.0107)、高血鉀 5.3% vs 12.7%(P=0.048)——與 `arts_program_Pitt_2013.md` 完全一致。
- FIND-CKD eGFR 斜率 −3.3 vs −4.0(差異 0.7,95% CI 0.3–1.1,P<0.001)——與 `FIND-CKD_NEJMoa2604625.md` 完全一致。
- Amazit 2015 分子機制數字(見發現三,數值本身正確)。
- Geller 2000 S810L 突變、spironolactone 於突變體轉為致效劑、懷孕惡化案例——與 `r2_Geller_2000.md` 一致。
- Fagart 2010 BR-4628「bulky, passive antagonist」原型概念——與 `r2_Fagart_2010.md` 一致。
- Coresh 2019 UACR 30% 下降 HR 0.83(0.74–0.94)/校正後 0.78(0.66–0.92),及「支持作為替代終點」之結論——與 `r2_Coresh_2019.md` 摘要/Implications 段落逐字呼應,非過度延伸。
- Filippatos 2023 全因死亡 HR 0.82(0.70–0.96,P=0.014)、CV 死亡 HR 0.82(0.67–0.99,P=0.040)、猝死 HR 0.75(0.57–0.996,P=0.046)、「大體上與代謝因子無關」之表述——與原文摘要幾乎逐字對應。
- Rossing 2022 SGLT2i 交互作用 P=0.46(CV)、P=0.29(腎臟)——與 `biomarker_Rossing_2022.md` 完全一致。
- Docherty 2025 LVEF 分層交互作用 P=0.70——與 `hf_finearts_Docherty_2025.md` 完全一致。
- Van 2026 FINEARTS-HF 主終點 rate ratio 0.84(0.74–0.95,P=0.007)、惡化 HF rate ratio 0.82(0.71–0.94);RALES/EMPHASIS-HF/EPHESUS/TOPCAT 各數字與適應症背書——與 `hf_finearts_Van_2026.md` 完全一致。
- Chimura 2026(N=6001,EMPEROR-Preserved 風險模型鑑別度、相對效益跨風險層一致)、Solomon 2024(NT-proBNP 中位數 1041 pg/mL,標記 📌 為 abstract-only 正確)、Lu 2026(猝死前 NT-proBNP 約 1800→2000、存活者 800→650、KCCQ-TSS 約降 8 分)——皆與對應本地全文一致。
- Verma 2026 之 CONFIDENCE 試驗數字(finerenone+empagliflozin 較 empagliflozin 單用多降 32%、較 finerenone 單用多降 29% 白蛋白尿;高血鉀頻率降低約 15%–20%)、指南建議 finerenone 與 GLP-1 RA 用於 CKD 合併糖尿病、高血鉀整數風險評分模型——皆與 `biomarker_Verma_2026.md` 逐字或近逐字對應。
- 表 1 各項藥理學比較(親和力排序、組織分布、輔因子招募模式、半衰期/代謝物、親脂性倍數、S810L 反應、適應症背書)——與 `molecular_Agarwal_2021.md`、`biomarker_Verma_2026.md`、`molecular_Kolkhof_2017.md` 交叉核對一致。

## Ghost Consensus 檢查

搜尋「許多研究」「多數證據」「普遍認為」「通常」「多項研究」「大量證據」「廣泛認為」「一致認為」「多數學者」等關鍵詞,**全文無命中**。文中所有多來源合併陳述(如「跨族群、跨器官、跨 LVEF、獨立於 SGLT2i 與血壓的一致性」,第 126 行)皆逐條列出具體試驗與引用來源(第 118–125 行的 1–5 點清單),非籠統宣稱,**未發現 ghost consensus**。

## Synthesis Overreach 檢查

第 148 行「當降壓幅度有限、卻在跨族群/跨器官/跨LVEF/獨立於SGLT2i的情境下一致觀察到效益時,最簡約的解釋即是『阻斷了MR相關的發炎–纖維化病理』」——此為作者明示的論證立場(「本文的立場」,第 12 行),且第 6 節「誠實承認的限制」已主動聲明缺乏頭對頭腎臟硬終點試驗、僅能由機制與各自安慰劑對照試驗間接推論。此為有適當 hedging 的 synthesis,**未達 overreach 標準**,判定通過。

## 時序檢查

本文引用之最新文獻為 2026 年發表(Verma 2026、Lu 2026、Chimura 2026、Van 2026),對照今日日期 2026-07-08,無 2026 年文獻引用 2027 年研究的情形,**未發現時序異常**。

---

## 總結

| 項目 | 結果 |
|---|---|
| Dead-link(檔名有標註但 References 無編號) | 1 件(必修)——`_prior_fidelio_figaro_extract.md` |
| 論斷對應(高權重數字逐一核對) | 全數通過,無 misattribution |
| Ghost consensus | 無命中 |
| Synthesis overreach | 無,已充分 hedge |
| 時序異常 | 無 |
| 格式一致性(References DOI 缺漏) | 1 件(待議)——ref #5 |
| Provenance 風險提示未承接 | 1 件(待議)——Amazit 2015 HTML 擷取警語 |

本文整體引用品質高,References 22 條與正文引用高度吻合,唯一必修項為 `_prior_fidelio_figaro_extract.md` 缺少對應編號書目條目,建議依上述選項 A 修正(改用已有的 FIDELIO/FIGARO 編號引用)最為簡潔。
