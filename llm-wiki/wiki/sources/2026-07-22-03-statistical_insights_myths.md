---
tags: [素材摘要, 統計方法學, 中介分析, 替代終點, 統計迷思]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/03-statistical_insights_myths.md
images: 0
image_paths: []
---

# 統計迷思與深度解讀 · 主題三（combination／mediation／短期替代終點的統計）

> 五個床邊最易誤讀的統計陷阱：中介比例的不對稱、P 值的沉默、替代終點的外推、「加成」不等於「超加成」、以及別把觀察性次組的 confounding 帶進隨機化結論。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/03-statistical_insights_myths.md
- **消化日期**：2026-07-22

## 核心觀點

1. **教學錨點**：以「相對風險 vs 絕對風險」為最古老的統計迷思錨點——同一個 HR 在不同基線風險的人身上換算出的絕對受益天差地別（主題四：statin RRR 29.2% 一致，但 ARR 從 1.5% 到 14.6%）。由此延伸出 combination 試驗特有的四個陷阱。

2. **迷思 1：中介的不對稱是機轉指紋，不是雜訊（🟡 exploratory）**。誤解是「combination 多降的 UACR 不就是兩藥各自壓球內壓、應該對稱嗎」。實際上 CONFIDENCE 因果中介分析（N=790 evaluable、690 進入 mediation）顯示方向不對稱：加 empagliflozin 的益處經急性 eGFR 中介 **28%（P=0.07）**，加 finerenone 僅 **5.2%（P=0.23）**。原文：combination 較 finerenone 多降的 29%「was partially mediated by the acute change in eGFR」，較 empagliflozin 多降的 32% 則「almost entirely independent of the acute eGFR change」。急性 eGFR 下降本身也不對稱：combination **−26.6**、finerenone **−22.1**、empagliflozin **−24.8**（P<0.001）。

3. **迷思 1 的誠實邊界**：原文自陳「Owing to the exploratory nature of the mediation analysis, wide CIs, and P values above 0.05, the results should be interpreted with a degree of caution」——**方向可信、精確點值不宜當硬數字宣讀**。臨床轉換：看到 finerenone 起始後 eGFR 只輕微 dip，不代表它沒在保護腎臟——它的保護本來就不寫在急性血流動力學這條路上。

4. **迷思 2：沉默不是清白（absence of evidence ≠ evidence of absence）**。誤解是「P=0.91／0.85 都不顯著，**證明**同步聯用不會多出高血鉀」。實際上兩個 P 值講的是「沒偵測到差異」。攤開絕對率：整體 113 人（14.5%）＝ combination **40/265（15.1%）**、finerenone **48/255（18.8%）**、empagliflozin **25/259（9.7%）**；相對 empagliflozin 的 aOR combination **2.69（1.46–4.96）**與 finerenone **2.56（1.42–4.59）幾乎重疊**——同步加 SGLT2i 後升鉀的 OR 沒有往下掉。

5. **迷思 2 的 power 限制（原文自承三點）**：finerenone 只讓血鉀升約 **+0.18 mEq/L**，「roughly one-third less than…spironolactone」，而「This smaller potassium excursion may have limited the opportunity to detect a mitigating effect of empagliflozin」；因此「the absence of a demonstrable reduction in hyperkalemia risk should be viewed as **hypothesis-generating rather than definitive**」。加上 180 天短試驗、事件數少（113 件）、主要終點是 UACR 而非高血鉀安全性。Wen 統合印證：combination vs finerenone 高血鉀 OR **1.09（0.52–2.28、I²=95.1%）**，CI 寬到 1 兩側都涵蓋，根本不是「等效」的證據。

6. **迷思 2 的床邊翻譯**：同步聯用時血鉀監測節奏**照 finerenone 單藥的規格走**（起始／增量後 4 週複測），不能因為加了 SGLT2i 就鬆手。

7. **迷思 3：180 天 UACR 到硬結局隔著一次外推**。CONFIDENCE 主要終點是 Day 180 的 log-UACR 相對變化，是替代終點。外推的正當性建立在外部證據：2019 年 41 試驗、29,979 人病人層級統合（median 3.4 年、3935 事件）顯示前 6 個月 ≥30% albuminuria 下降對應長期腎複合終點風險降 **27%（HR 0.73；0.67–0.81）**；CONFIDENCE 過半受試者跨過門檻（very high 層 70.6%）。但兩個硬邊界：(1) 硬終點 Phase 3 估計需隨機化約 **41,000 人**；(2) Wen 的 TSA 顯示 combination vs SGLT2i 單藥的 mortality（OR 0.73；0.47–1.13）、MACE（0.77；0.55–1.08）、MAKE（0.87；0.58–1.31）皆不顯著，累積 Z 曲線「did not cross trial sequential monitoring boundaries for benefit nor enter futility zone」。

8. **迷思 3 的床邊語言**：把 combination 定位成「更快讓 UACR 進入低風險帶、爭取時間」，而非「已證明多救多少顆腎」。

9. **迷思 4：「additive」還是「over-additive」——三個層次要分清**。(a) **preclinical**：高血壓終末器官損傷大鼠中，低劑量 combination 產生「premature, sustained, and over-additive reduction in albuminuria」，7 週存活率也顯著較高——動物、劑量與物種都需外推。(b) **臨床「比單藥好」**：combination vs finerenone LSMR **0.71（0.61–0.82）**、vs empagliflozin **0.68（0.59–0.79）**，皆 P<0.001——證明的是「優於各單藥」。(c) **統計上的『超加成』**：需 2×2 factorial 設計檢定「合併效果 > 兩單藥效果的加總／相乘」；**CONFIDENCE 是三臂平行、並非為 super-additivity 的正式交互檢定而設計，也沒有報這個 interaction P 值**。

10. **文獻裡的 P_interaction 是另一回事**：Vaduganathan 測的是「combination 相對益處在 KDIGO 風險層間是否一致」，得 P_interaction >.05（very high 層 LSMR 0.72／0.75），檢定的是跨風險層一致性、不是超加成；且該分析明載「No adjustment for multiple comparisons was made」。**站得住的說法是「明確優於任一單藥、且跨風險層一致」，而非浮誇的「協同 synergy」**——那個詞的最強證據仍在動物模型（🔴）。

11. **迷思 5：結論要放回它的設計**。誤解是「FIDELITY 看到基線用 SGLT2i 者高血鉀較少（10.3% vs 14.3%），CONFIDENCE 沒看到，八成是 CONFIDENCE 有問題」。實際上兩者不矛盾，差別在設計與時序：FIDELITY 的 SGLT2i 亞組雖為 prespecified pooled analysis，但「是否使用 SGLT2i」非隨機分派——基線用者本就腎功能較好（mean eGFR **66.3 vs 57.0**）、UACR 較低（median **448 vs 521 mg/g**）、GLP-1RA 使用率高約三倍（**19.0% vs 6.4%**），典型 **confounding by indication**，只能看 P_interaction。

12. **證據階層的床邊用法**：當隨機化證據（CONFIDENCE）與觀察性訊號（FIDELITY 亞組）方向不一致時，**以隨機化為準**，把觀察性訊號降級為「可能的時序假說」。兩者的時序不同，正好被 FIVE-STAR 的 P-interaction 0.02（未用 SGLT2i **+0.37** vs 已用 **+0.13 mEq/L**）串起來——降鉀效應可能需要 SGLT2i 先「適應」一段時間，但仍需 Sinclair 呼籲的三臂 sequencing RCT 證實（🔴）。

13. **統計素養檢查表（查房一頁）**：看到亮眼相對降幅→問要幾步外推；看到「不顯著」的安全性 P 值→問這分析有沒有 power、主終點是不是它；看到「combination 比單藥好」→問是「優於單藥」還是「正式檢定的超加成」；看到 mediation 百分比→問是不是 exploratory、CI 多寬；看到 P_interaction→問它檢定的是一致性、加成還是效果修飾、校正多重了嗎；看到觀察性亞組組間差→問有無 confounding by indication。

## 關鍵概念

[[中介分析]]、[[三的法則（rule of three）]]、[[替代終點]]、[[over-additive 效應]]、[[over-additive 效應]]、[[confounding by indication]]、[[交互作用檢定]]、[[trial sequential analysis]]、[[相對風險與絕對風險]]、[[FIVE-STAR]]

## 與其他素材的關聯

- 為主題三主文的統計深度解讀附冊 → [[2026-07-22-03-03_fourth_pillar_or_early_combination]]
- 數字出處的完整脈絡 → [[2026-07-22-03-confidence_trial_deep_dive]]、[[2026-07-22-03-discussion_controversies_endpoint_hyperkalemia_cost]]
- over-additive 語意辨析的另一版本 → [[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]
- subgroup 旁證的原始效應量 → [[2026-07-22-03-real_world_combination_logic_indirect_evidence]]
- 教學錨點（statin RRR 29.2% / ARR 1.5–14.6%）引自主題四的相對 vs 絕對方法學檔 <!-- confidence: EXTRACTED -->

## 原文精彩摘錄

> 把 mediation 想成「拆帳單」：加 empa 的帳單裡約三成是「血流動力學（壓球內壓）」這個項目，加 finerenone 的帳單裡這個項目幾乎是零。

> 把 P=0.91／0.85 正確翻譯成「**同步起始 SGLT2i 並沒有幫你把 finerenone 的高血鉀抵消掉**」，而不是「聯用很安全不用管鉀」。

> 臨床決策不需要「超加成」成立——「combination 比兩個單藥各自都好、且不論病人腎風險高低都好」已足以支持「不必等到極高風險才聯用」。但把「over-additive」當成已被人體正式檢定的統計結論來衛教，會超出資料能承擔的範圍。

## 相關頁面

- [[2026-07-22-03-03_fourth_pillar_or_early_combination]]
- [[2026-07-22-03-confidence_trial_deep_dive]]
- [[2026-07-22-03-discussion_controversies_endpoint_hyperkalemia_cost]]
- [[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]
- [[2026-07-22-03-real_world_combination_logic_indirect_evidence]]
