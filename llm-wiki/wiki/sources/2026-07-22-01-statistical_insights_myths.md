---
tags: [素材摘要, 統計方法學, 中介分析, 相對vs絕對風險, 替代終點]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/01-statistical_insights_myths.md
images: 0
image_paths: []
---

# 統計迷思與深度解讀 · 主題一

> 從分子數字（親和力、選擇性倍數）或生物標記（UACR、NT-proBNP、風險分數）推論「病人能拿到多少臨床好處」時，統計上有四個量綱錯置的坑；校準尺是最古老的相對風險 vs 絕對風險。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/01-statistical_insights_myths.md
- **消化日期**：2026-07-22

## 核心觀點

1. **錨點：同一個 HR，NNT 可以差 12 倍（🟢/🟡）**。Chimura 的 FINEARTS-HF 次分析（6001 名 HFmrEF/HFpEF）用 EMPEROR-Preserved 風險模型分五等分，finerenone 相對效果跨層一致（Q1→Q5 的 HR 為 0.93、1.04、0.82、0.81、0.88，P for interaction = .68）；但最低風險 Q1 的絕對下降僅 3.7 per 1000 person-years（NNT 272），最高風險 Q5 為 43.0 per 1000 person-years（NNT 23）📄[biomarker_Chimura_2026.md]。「HR 不變」不是「人人一樣受益」的證據，恰恰保證高風險病人的絕對受益更大。

2. **迷思一：「500-fold 選擇性」不是效益倍數（🔴→🟢）**。選擇性倍數是藥理效價比，量的是「這個分子多偏好 MR、多不去碰其他受體」，與硬終點效益是不同量綱。Kolkhof 原文把效價與選擇性分開講：finerenone「is at least as potent as spironolactone and even more selective (at least 500-fold toward MR) than eplerenone」，該選擇性是對照 65 個受體與離子通道（含 L-type Ca²⁺ channel）測出 📄[molecular_Kolkhof_2017.md]。實際效價 IC50 58 ± 9 vs 74.0 ± 15 nM（Kd 1.52 ± 0.01 nM）——只差約 1.3 倍 📄[molecular_Amazit_2015.md]。esaxerenone 的「at least a 1000-fold higher selectivity」同理。

3. **高選擇性的正確臨床翻譯**是副作用譜更乾淨（不碰雄激素／黃體素受體 → 少男性女乳症）與分子行為可預測（對 S810L 維持嚴格拮抗）；「有多少心腎保護」只能由 RCT 的 HR/NNT 回答。

4. **迷思二：「BP-independent」不是「沒降血壓」（🟡）**。它有降壓——FIDELITY 第 4 個月 SBP −3.2 vs 安慰劑 +0.5 mmHg 📄[biomarker_Agarwal_2022.md]——只是幅度不大。「獨立」是中介分析的結論。

5. **中介分析的具體數字**：Agarwal 2026 用 FIDELITY 個體資料（n = 12,143）做 causal mediation，第 4 個月 finerenone 降 UACR 32.2%、降 SBP 3.6 mmHg；四個候選中介裡只有 UACR 中介 39%（95% CI 7 to 71）、SBP 中介 21%（3 to 40），體重與血鉀不中介，兩者合計中介 50%（95% CI 21 to 100）📄[biomarker_Agarwal_2026.md]。先前單獨分析中 UACR 單獨中介 37%、SBP 以 time-varying 法估 12.6%。臨床意涵：不能靠加一顆降壓藥複製 finerenone 的效益，因為約 80% 走別條路；但 21% 也不是 0%。

6. **迷思三：預後 ≠ 療效預測（🟡）**。鑑別度回答「模型能不能排出誰會出事」，與「finerenone 對誰的相對效果更大」是兩個獨立問題。Chimura 模型鑑別度好——Q5 vs Q1 事件 HR 高達 10.49（95% CI 8.14–13.52），CV death 更達 13.47，且優於單用 NT-proBNP；但治療效果跨五分位是平的（P for interaction = .68）📄[biomarker_Chimura_2026.md]。它推出的是絕對受益梯度（NNT 272 → 23），不是相對療效修飾。

7. **風險標記 vs 中介的區分**：Lu 2026 顯示猝死前 6 個月 NT-proBNP 由約 1800 升到 2000 pg/mL，存活者則由約 800 降到 650 pg/mL 📄[biomarker_Lu_2026.md]——這是縱向風險標記軌跡，作者明言為 population-level、hypothesis-generating，不等於「壓低 NT-proBNP 就等量換到存活」。

8. **迷思四：「至少與 spironolactone 相當」不是等效硬終點（🔴）**。ARTS 是 phase II，主終點是血清鉀變化，生物標記全屬 only exploratory；原文明寫 part B「showed no significant overall treatment effect on BNP, NT-proBNP, or urinary albumin:creatinine ratio (UACR) (P > 0.05), so P-values for individual treatment group comparisons were not calculated, and the treatment groups were analysed only descriptively」📄[arts_program_Pitt_2013.md]。其樣本量是為偵測 K⁺ 差 0.26 mmol/L 而算（80% power）。

9. **ARTS-HF 同理**：phase 2b，主終點「NT-proBNP 下降 >30% 的比例」，eplerenone 37.2% vs finerenone 各劑量 30.9–38.8%（P = 0.42–0.88）；臨床複合 HR 0.56（0.35–0.90）是探索性、nominal P，原文自陳「not designed to detect statistical significant differences」，並提醒「changes in natriuretic peptides by several drugs were not related to improved outcome in clinical trials」📄[arts_hf_Filippatos_2016.md]。「至少相當」是 absence of evidence，不是 evidence of absence。

10. **finerenone 硬終點地位的來源**是 FIDELIO/FIGARO/FIDELITY 與 FINEARTS-HF 的安慰劑對照，而非任何對 spironolactone/eplerenone 的頭對頭等效證明——本主題全無此類長期硬終點對頭資料（**尚待驗證**）。原檔另附一頁式「統計素養檢查表」供查房／簡報使用。

## 關鍵概念

- [[相對風險與絕對風險]]
- [[NNT]]
- [[中介分析]]
- [[替代終點]]
- [[治療效應異質性]]
- [[UACR]]
- [[NT-proBNP]]
- [[FIDELITY]]
- [[FINEARTS-HF]]
- [[ARTS-DN]]

## 與其他素材的關聯

- 與 `01-01_finerenone_not_just_safer_spironolactone.md` 是**校正／反駁**關係：主文引用的 ARTS「至少相當」、FINEARTS-HF 風險分層一致、BP-independent 等表述，本檔逐一指出正確與錯誤的讀法邊界。<!-- confidence: EXTRACTED -->
- 與 `01-mr_receptor_dissociation_residence_time.md` 互補：迷思一所需的「效價只差 1.3 倍」原始數字（IC50 58 vs 74 nM）正是受體動力學檔的核心錨點。<!-- confidence: INFERRED -->
- 迷思二的中介百分比（UACR 39%、SBP 21%、合計 50%）是主題二「UACR 是伴隨型生物標記還是機轉連結替代終點」的直接答案來源。<!-- confidence: INFERRED -->
- 本檔提及 ARTS-DN 的 UACR 21–38% 劑量反應（`arts_program_Bakris_2015.md`）僅列於語料清單、未在正文展開數字脈絡。<!-- confidence: AMBIGUOUS -->

## 原文精彩摘錄

> 「HR 不變」不是「人人一樣受益」的證據，恰恰相反，它保證高風險病人的絕對受益更大。看到「跨亞群一致」的漂亮森林圖，正確反應是去算病人的基線絕對事件率，而不是把 HR 當成每個人都能拿到的折扣。

> 把 500-fold 當作「療效證書」是把分子藥理學的尺拿去量臨床結局——量綱錯了。

> 「至少相當」在統計上是沒有證明差異（absence of evidence），不是證明沒有差異（evidence of absence）——尤其在 power 只夠比血鉀的試驗裡。

## 相關頁面
